# Maintainer: Jerome Gravel-Niquet <jeromegn@gmail.com>

pkgname="flyctl-bin"
pkgver="0.0.251"
pkgrel="1"
pkgdesc="Command line tools for fly.io services"
arch=("x86_64")
url="https://fly.io"
license=("Apache")
depends=()
provides=("flyctl")
conflicts=("flyctl")
source=("$pkgname-0.0.251.tgz::https://github.com/superfly/flyctl/releases/download/v0.0.251/flyctl_0.0.251_Linux_x86_64.tar.gz")
sha256sums=('4e2641b30bc0f069ab796a94ef7a5a664e72baf51fc5fd307718e29d7b964edc')

package() {
    mkdir -p "$pkgdir/usr/bin"
    ln -s flyctl "$pkgdir/usr/bin/fly"
    install -m755 flyctl "$pkgdir/usr/bin"
}

