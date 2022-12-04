#Maintainer: silent robot (d3signr@gmail.com)

pkgname=salientos-scripts-kde
pkgver=1.0
pkgrel=0
pkgdesc='Salient OS Install Scripts'
url="https://github.com/salientos/"
arch=('any')
license=('GPL3')
makedepends=('git')
depends=()
conflicts=('salientos-scripts-xfce')
provides=("${pkgname}")
options=(!strip !emptydirs)

source=('chrooted_post_install.sh'
		'post_install.sh')

sha512sums=('a2423a3fd5d94ded70e48a837b429b6f5644cbb4671213528e0aa392d251b3d81fd82c3b1e5557378a020378da3ef7a77b03c9cec99c46a6d3183119a82e3b28'
            '83956261269ee95b41d49f082a683e74324e668608159e014a6c33c26f4bd5672a0e6589e2ccaf1457b11a6d6aafe1ab2b6f327c013ce0f707ce74a7d9699891')

package() {
	local bin=${pkgdir}/usr/bin
	install -Dm755 chrooted_post_install.sh 	${bin}/chrooted_post_install.sh
	install -Dm755 post_install.sh 				${bin}/post_install.sh
}
