# Maintainer: Jerome Gravel-Niquet <jeromegn@gmail.com>

pkgname="flyctl-bin"
pkgver="0.0.464"
pkgrel="1"
pkgdesc="Command line tools for fly.io services"
arch=("x86_64")
url="https://fly.io"
license=("Apache")
depends=()
provides=("flyctl")
conflicts=("flyctl")
source=("$pkgname-0.0.464.tgz::https://github.com/superfly/flyctl/releases/download/v0.0.464/flyctl_0.0.464_Linux_x86_64.tar.gz")
sha256sums=('8254ad2c9cdb908713b4ea8294cb4035e87afcb2672da632e4fedde92bff3a40')

package() {
    mkdir -p "$pkgdir/usr/bin"
    ln -s flyctl "$pkgdir/usr/bin/fly"
    install -m755 flyctl "$pkgdir/usr/bin"
}
