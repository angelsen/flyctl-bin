# Maintainer: Jerome Gravel-Niquet <jeromegn@gmail.com>
# Co-maintainer: Fredrik Angelsen <fredrikangelsen@gmail.com>

pkgname="flyctl-bin"
pkgver="0.3.31"
pkgrel="2"
pkgdesc="Command line tools for fly.io services"
arch=("x86_64")
url="https://fly.io"
license=("Apache")
depends=()
provides=("flyctl")
conflicts=("flyctl")
_name=flyctl
source=("$pkgname-$pkgver.tgz::https://github.com/superfly/flyctl/releases/download/v${pkgver}/${_name}_${pkgver}_Linux_x86_64.tar.gz")
sha256sums=('144b82f13a2406080c01fc07bc871516d0f1204b054db65c75c58a649fdb166f')

package() {
    mkdir -p "$pkgdir/usr/bin"
    install -m755 "$srcdir/$_name" "$pkgdir/usr/bin/$_name"
    ln -s "$pkgdir/usr/bin/$_name" "$pkgdir/usr/bin/fly"
}
