# Maintainer: Guten Ye

pkgname="user-gnote-daemon"
pkgver=0.1
pkgrel=4
pkgdesc="a user daemon for gnote-plugin. READ https://github.com/GutenYe/user-daemon-system FIRST"
arch=("i686" "x86_64")
url="https://github.com/GutenYe/gnote-plugin"
license=("MIT")
depends=("user-daemon-system-git")
source=("rc.gnote")

package() {
  cd $srcdir

	install -Dm755 rc.gnote $pkgdir/home/$USER/etc/rc.d/gnote

  chown $USER:$USER -R $pkgdir/home/$USER
}

# vim:set ts=2 sw=2 et:
md5sums=('38b24dd52b3c8ef0b2df4bc5317a03c8')
