# Maintainer: DarkXero <info@techxero.com>
pkgname=calamares-config
_destname1="/etc"
pkgver=22.02
pkgrel=5
pkgdesc="calamares Config for XeroLinux KDE"
arch=('any')
url="https://github.com/xerolinux"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=('alci-calamares-config' 'alci-calamares-config-pure' 'alci-calamares-config-btrfs')
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${srcdir}/${pkgname}/creds.sh
	rm ${srcdir}/${pkgname}/push.sh
	rm ${srcdir}/${pkgname}/README.md
	rm ${srcdir}/${pkgname}/PKGBUILD
}
