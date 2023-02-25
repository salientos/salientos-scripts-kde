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

sha512sums=('ef1fc695e291ba3f15ac6de65563d495d447c98df5192e97aad31dcdfcf91e8b7abafc0ca01669b39cc7d8b85582ff0340d382f840ed543414dbecf46510408a'
            '6dfffbc970e0a37c3f2b7cdf78d144c9da5677e074ae88f494bbb5d03ef0799fbd9041987ad756b8fd0a7c60b4bec80ec5869471fba9a9cac52b78265bcf01cd')

package() {
	local bin=${pkgdir}/usr/bin
	
	install -Dm755 chrooted_post_install.sh 	${bin}/chrooted_post_install.sh
	install -Dm755 post_install.sh 				${bin}/post_install.sh
	
	chmod +x ${bin}/chrooted_post_install.sh
	chmod +x ${bin}/post_install.sh
}
