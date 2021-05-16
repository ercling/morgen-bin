# Maintainer: Oleksandr Mykhailiuta <ercling@gmail.com>
# Upstream: Morgen AG <connect@morgen.so>

pkgname='morgen-bin'
pkgver='2.0.7'
_pkgver='2.0.7'
pkgrel='1'
pkgdesc='Morgen Calendar. Faster, lighter and more robust. Evolution of MineTime'
arch=('x86_64')
url='https://morgen.so/'
license=('custom')
depends=('gtk3' 'libnotify' 'nss' 'libxss' 'libxtst' 'xdg-utils' 'at-spi2-core' 'util-linux-libs' 'libappindicator-gtk3' 'libsecret')
provides=('morgen')
# source=("https://downloads.bitwig.com/stable/${_pkgver}/bitwig-studio-${_pkgver}.deb")
source=("https://dl.todesktop.com/210203cqcj00tw1/linux/deb/x64")
sha256sums=('1786713ed48d666fa98f8bf4dc99734e1c1cb1fa4f608987d1232bc551e91fa7')

package() {
  # Unpack package contents
  tar -xJC "${pkgdir}" -f data.tar.xz

  install -Dm 755 "${startdir}"/morgen "${pkgdir}"/usr/bin/morgen

  # Install license
#   install -D -m644 ${pkgdir}/opt/bitwig-studio/EULA.rtf ${pkgdir}/usr/share/licenses/${pkgname}/LICENSE
}
