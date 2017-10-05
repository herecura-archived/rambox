#Maintainer: Janek Thomaschewski <janek@jbbr.net>

pkgname=rambox
pkgver=0.5.13
pkgrel=1
pkgdesc='Free and Open Source messaging and emailing app that combines common web applications into one.'
arch=('i686' 'x86_64')
depends=('alsa-lib' 'desktop-file-utils' 'gconf' 'gtk2' 'libnotify' 'libxtst' 'libxss' 'nss')
url='http://rambox.pro/'
license=('MIT')
source_i686=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-ia32.rpm")
source_x86_64=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-x64.rpm")

sha512sums_i686=('84a650905cae1c2b487d48a6debfb1be66a925fc9dee524528ec4bf2c5f40142981553db670d87c14dceb1943dc3d6e22f417aaf6ef08ea82571356695b54a00')
sha512sums_x86_64=('57181551a62d4e28921412c2dbd43161a53cc41db86e8b5b6cad2c93ee1b7e5aab15a402fdf25dfbab91fa4e829f7d60d4ab7c8849564bdd76f89eabee5d9deb')

package() {
    cp -a {opt,usr} "$pkgdir"
    install -dm755 "$pkgdir/usr/bin"
    ln -sf /opt/Rambox/rambox "$pkgdir/usr/bin/rambox"
}
