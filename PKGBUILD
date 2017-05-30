#Maintainer: Janek Thomaschewski <janek@jbbr.net>

pkgname=rambox
pkgver=0.5.9
pkgrel=1
pkgdesc='Free and Open Source messaging and emailing app that combines common web applications into one.'
arch=('i686' 'x86_64')
depends=('alsa-lib' 'desktop-file-utils' 'gconf' 'gtk2' 'libnotify' 'libxtst' 'libxss' 'nss')
url='http://rambox.pro/'
license=('MIT')
source_i686=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-ia32.rpm")
source_x86_64=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-x64.rpm")

sha512sums_i686=('e0995ee3ab1c0fdabd316db51442ac24d5688a0963890ac3b5f314440cddc96637bf4fc8bcc562dd2ba0448a2a8d92e1d72281ba34ef983f95046098214a2975')
sha512sums_x86_64=('39d68627754adbcec8559b16be121313a6b07d0b5e8eb402ed4c26b9fd17d671a29480eccdc5e9525c2ec3f6ac1efcbeb1cc908f28a4429fa6fd8d42eabc5c06')

package() {
    cp -a {opt,usr} "$pkgdir"
    install -dm755 "$pkgdir/usr/bin"
    ln -sf /opt/Rambox/rambox "$pkgdir/usr/bin/rambox"
}
