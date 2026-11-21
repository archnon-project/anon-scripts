pkgname=archnon-project
pkgver=4.0.1
pkgrel=1
pkgdesc="A collection of bash scripts for extreme anonymity and privacy on Linux. Works for systemd, runit and open-rc. Includes i2pd, tor and nftables."
arch=('any')
url="https://github.com/archnon-project/anon-scripts"
license=('GPL-3.0-or-later')
makedepends=('git')
depends=('bash')
source=("git+https://github.com/archnon-project/anon-scripts.git")
sha256sums=('SKIP')

package() {

  main="$srcdir/anon-scripts"

  cd $main

  install -dm755 "$pkgdir/usr/local/bin"

  mini_path="$pkgdir/usr/local/bin"

  if [ -f README.md ] && [ -f LICENSE ]; then
    install -Dm644 README.md "$pkgdir/usr/share/doc/$pkgname/README.md"
    install -Dm644 LICENSE "$pkgdir/usr/share/license/$pkgname/LICENSE"
  fi

  scripts=(archnon mars neptune saturn uranus)

  for i in "${scripts[@]}"; do
    install -Dm755 "$i" "$mini_path/$i"
  done

}
