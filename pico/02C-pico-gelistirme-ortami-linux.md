# Raspberry Pi Pico Linux Geliştirme Ortamı
Bu dökümanda Linux tabanlı işletim sistemlerinde Pico geliştirme ortamı ile ilgili bilgilere ulaşabilirsiniz.

# Pico C/C++ SDK için Geliştirme Ortamı
Raspberry tarafından geliştirilen ve Pico kartımız ile C/C++ ile yazılım geliştirmemizi sağlayan Pico SDK'yı kullanabilmek için sistemimizde:
- cmake
- arm-none-eabi-gcc
- git 

paketleri bulunmalıdır.

Bu paketlerin kurulumu Debian tabanlı dağıtımlarda:
`sudo apt install cmake gcc-arm-none-eabi git build-essential`

Fedora - RedHat tabanlı dağıtımlarıda:
`sudo dnf install cmake arm-none-eabi-gcc git`

Arch tabanlı dağıtımlarda:
`sudo pacman -S cmake arm-none-eabi-gcc git`

## Pico SDK'nın Klonlanması
Pico SDK dosyalarını isterseniz 'git' kullanarak, isterseniz direkt olarak Github üzerinden indirerek temin edebilirsiniz. Bizim tavsiyemiz 'git' kullanarak pico-sdk deposunu sisteminizde kolayca bulabileceğiniz bir konuma klonlamanızdır. 

`git clone https://github.com/raspberrypi/pico-sdk`

Pico SDK'yı aynı zamanda [pico-sdk deposuna](https://github.com/raspberrypi/pico-sdk) gidip yeşil 'Code' butonuna tıklayıp 'Download ZIP'i seçerek de indirebilirsiniz. 

### ! Pico SDK'nın çıkartılmış olduğu klasörün yolu ,örnek ~/Belgeler/pico-sdk, geliştirme sırasında gerekli olduğu için bir yere not edilmelidir.

## IDE Kurulumu
Pico SDK ile yapacağınız geliştirmelerde önerilen IDE Visual Studio Code'tur. İsterseniz Microsoft tarafından yayınlanan ve içinde veri toplama(telemetry) bulunan versiyonunu, isterseniz VSCodium versiyonunu kurabilirsiniz. Arch tabanlı dağıtım kullanıcıları dağıtımlarının kendi sağladığı `code` paketini kurabilirler.

[Visual Studio Code](https://code.visualstudio.com/)

[VSCodium](https://vscodium.com/)

IDE olarak başka yazılımları da tercih edebilirsiniz. Ama yazılımınızı Debug modunda incelemek için Visual Studio Code ve türevi IDE'ler kullanmanız gerekmektedir. 

# Micropython için Geliştirme Ortamı
Micropython, mikrodenetleyici kartlar için tasarlanmış, normal Python'a göre daha hızlı çalışan ve daha az kaynak kullanan bir [Python implementasyonudur](https://wiki.python.org/moin/PythonImplementations). Micropython paketi çeşitli dağıtımlarda paketlenmiş halde bulunmaktadır. Dağıtımınızda Micropython paketi mevcutsa bu paketi kullanmanız tavsiye edilir.

- Arch Linux:   [AUR](https://aur.archlinux.org/packages/micropython/) paketi `yay` veya `paru` AUR yardımcısı ile derlenebilir.    

- Debian:       micropython paketi şuanda sadece Debian Sid(unstable) versiyonunda bulunmaktadır. Yakın bir zamanda yayınlanacak olan Debian 11(bullseye) versiyonunda dahil edilebilir. Debian Sid kullanıcıları `sudo apt install micropython` komutu ile paketi kurabilirler. 

- Fedora:       micropython paketi resmi depolarda bulunmaktadır. `sudo dnf install micropython` 

- Ubuntu:       20.04 ve 20.10 depolarında micropython paketi bulunmaktadır. `sudo apt install micropython` 

- openSUSE      micropython paketi [devel:languages:python](https://build.opensuse.org/project/show/devel:languages:python) resmi deposunda bulunmaktadır. [Bu adresten](https://software.opensuse.org//download.html?project=devel%3Alanguages%3Apython&package=micropython) kurulum talimatlarına ulaşılabilir. 

Güncel paket listesi: https://repology.org/project/micropython/versions

Eğer yukarıda belirtilen dağıtımları kullanmıyorsanız ve dağıtımınız size micropython paketini sağlamıyorsa micropython'ın resmi Github adresindeki talimatları izleyerek derleyebilirsiniz.
https://github.com/micropython/micropython

## Micropython için IDE Kurulumu
Pico geliştirmesi için önerilen IDE Thonny'dir. Thonny Tkinter arayüz kütüphanesini kullanan, Python'la yazılmış basit bir Python IDE'sidir. Thonny paketi çoğu dağıtımın resmi deposunda bulunmaktadır.

- **Arch Linux**: [AUR](https://aur.archlinux.org/packages/thonny/) `yay -S thonny`

- **Debian**: `sudo apt install thonny`

- **Fedora**: `sudo dnf install thonny`

- **Ubuntu**: `sudo apt install thonny`

- **openSUSE**: thonny paketi [Education](https://build.opensuse.org/project/show/Education) resmi deposunda mevcuttur.
