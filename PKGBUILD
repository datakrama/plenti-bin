# Maintainer: A. Husen <hello@husen.id>
pkgname=plenti-bin
_pkgname=plenti
pkgver=0.4.17
pkgrel=2
pkgdesc="Static Site Generator with Go backend and Svelte frontend"
arch=('x86_64')
url="https://github.com/plentico/plenti"
license=('APACHE')
provides=('plenti')
conflicts=('plenti')
source=("${_pkgname}-${pkgver}.tar.gz::${url}/releases/download/v${pkgver}/plenti_${pkgver}_Linux_64-bit.tar.gz")
sha512sums=('b17a6943b4cf46e9266bc08ccfb8a6646e642047fabc2c63e12e45205f85c499b49f775713609af6a6a1c48bec84955b41704facfb9fbc8aac16934154f1cac4')

package() {
    cd "$srcdir"

    install -Dm755 $_pkgname		"${pkgdir}/usr/bin/${_pkgname}"

    install -Dm644 "README.md"		"$pkgdir/usr/share/doc/${_pkgname}/README.md"

    install -Dm644 "LICENSE"		"$pkgdir/usr/share/licenses/${_pkgname}/LICENSE"
}
