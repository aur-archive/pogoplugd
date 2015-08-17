# Maintainer: Sara <sara at archlinux dot us>

pkgname=pogoplugd
pkgver=1.0
pkgrel=2
pkgdesc="Run pogoplugfs as a daemon with a specified user"
arch=('i686' 'x86_64')
url="http://www.pogoplug.com"
license=('custom')
depends=('bash' 'pogoplugfs')
source=('pogoplugd' 'pogoplugd.conf.d')
backup=('etc/conf.d/pogoplugd')
md5sums=('573a5f700806328316341f3060981e57'
         '82992730ac65d605e3212fb42a16dea1')

package() {
  cd "${srcdir}"
  install -Dm755 "${srcdir}"/pogoplugd "${pkgdir}"/etc/rc.d/pogoplugd
  install -Dm644 "${srcdir}"/pogoplugd.conf.d "${pkgdir}"/etc/conf.d/pogoplugd
}

# vim:set ts=2 sw=2 et:
