## Raspberry Pi Pico Linux Geliştirme Ortamı
Bu dökümanda Linux tabanlı işletim sistemlerinde Pico geliştirme ortamı ile ilgili bilgilere ulaşabilirsiniz.

## Pico C/C++ SDK için Geliştirme Ortamı
Raspberry tarafından geliştirilen ve Pico kartımız ile C/C++ ile yazılım geliştirmemizi sağlayan Pico SDK'yı kullanabilmek için sistemimizde:
- cmake
- arm-none-eabi-gcc
- git 

paketleri bulunmalıdır.

Bu paketlerin kurulumu Debian tabanlı dağıtımlarda:
`sudo apt install cmake arm-none-eabi-gcc git build-essential`

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
Pico SDK ile yapacağınız geliştirmelerde önerilen IDE Visual Studio Code'tur. İsterseniz Microsoft tarafından yayınlanan ve içinde veri toplama(telemetry) bulunan versiyonunu, isterseniz VSCodium versiyonunu kurabilirsiniz. Arch tabanlı dağıtım kullanıcıları dağıtımlarının kendi sağladığı `code` paketini kurabilir.

[Visual Studio Code](https://code.visualstudio.com/)

[VSCodium](https://vscodium.com/)

IDE olarak başka yazılımları da tercih edebilirsiniz. Ama yazılımınızı Debug modunda incelemek için Visual Studio Code ve türevi IDE'ler kullanmanız gerekmektedir. 


