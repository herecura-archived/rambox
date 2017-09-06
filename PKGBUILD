#Maintainer: Janek Thomaschewski <janek@jbbr.net>

pkgname=rambox
pkgver=0.5.11
pkgrel=1
pkgdesc='Free and Open Source messaging and emailing app that combines common web applications into one.'
arch=('i686' 'x86_64')
depends=('alsa-lib' 'desktop-file-utils' 'gconf' 'gtk2' 'libnotify' 'libxtst' 'libxss' 'nss')
url='http://rambox.pro/'
license=('MIT')
source_i686=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-ia32.rpm")
source_x86_64=("https://github.com/saenzramiro/rambox/releases/download/$pkgver/Rambox-$pkgver-x64.rpm")

sha512sums_i686=('64c0ae65047dae654f760caeb4187976b23201177559d5b4c5e72362a0d72860e5c135fc73ed63131f17e884813b103389e467a912d3713f88dd4f4bd6792ad0')
sha512sums_x86_64=('236cb9d89caed538e64ca3147ed381d08a63cc224c4d1483cd95e83616272fd75d960aeecf5af84d34e4f3658bcb56f13257d8c9c509f774dd934f3adf93375c')

package() {
    cp -a {opt,usr} "$pkgdir"
    install -dm755 "$pkgdir/usr/bin"
    ln -sf /opt/Rambox/rambox "$pkgdir/usr/bin/rambox"
}
