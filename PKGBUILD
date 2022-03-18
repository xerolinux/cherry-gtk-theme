# Maintainer: DarkXero <info@techxero.com>
pkgname=cherry-gtk-theme
_destname1="/"
pkgver=0.1.0
pkgrel=1
pkgdesc="Cherry GTK Theme for XeroLinux"
arch=('any')
url="https://github.com/xerolinux"
license=('GPL3')
makedepends=('git')
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${srcdir}/${pkgname}/creds.sh
	rm ${srcdir}/${pkgname}/push.sh
	rm ${srcdir}/${pkgname}/PKGBUILD
}
