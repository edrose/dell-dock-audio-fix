# Maintainer: Ed Rose <ed@edrose.net>
pkgname=dell-dock-audio-fix
pkgver=1.0
pkgrel=1
pkgdesc="A fix for audio on Dell WD15 and TB15 Docks"
arch=('x86_64')
url=""
license=('unknown')
depends=('pulseaudio')
install=
changelog=
source=("91-pulseaudio.rules"
	"dell-dock-wd15-usb-audio.conf")
md5sums=('9e734a028693c944b1fe090ca4aeab3c'
	 '31745df6bd23bfd756486ef2255744c4')

package() {
	cd "${srcdir}"
	mkdir -p $pkgdir/usr/lib/udev/rules.d
	install 91-pulseaudio.rules "$pkgdir/usr/lib/udev/rules.d/91-pulseaudio.rules"
	mkdir -p $pkgdir/usr/share/pulseaudio/alsa-mixer/profile-sets
	install dell-dock-wd15-usb-audio.conf "$pkgdir/usr/share/pulseaudio/alsa-mixer/profile-sets/dell-dock-wd15-usb-audio.conf"
}
