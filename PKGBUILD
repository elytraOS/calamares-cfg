# Original Maintainer: DarkXero <info@techxero.com>
# Maintainer: Yashodhan Sawardekar <rasenkai99@gmail.com>
pkgname=calamares-cfg
_destname1="/etc"
pkgver=23.03
pkgrel=3
pkgdesc="calamares Config for elytraOS"
arch=('any')
url="https://github.com/elytraOS"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=('calamares-config-dev')
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${srcdir}/${pkgname}/README.md
	rm ${srcdir}/${pkgname}/PKGBUILD
}
