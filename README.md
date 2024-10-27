# ubuntu-kurulum

## Burada Ubuntu 24.04'ü kurmak için kapsamlı bir kılavuz bulacaksınız. 
[* 1. Ubuntu sistem gereksinimleri](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#SysReq) <br/>
[* 2. Ubuntu'yu yüklemeye hazırlanıyor](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#Prep) <br/>
[    ** 2.1 Görüntünün indirilmesi](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#LoadISO) <br/>
[  ** 2.2 Görüntüyü bir USB belleğe yazma](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#WriteISO) <br/>
[  ** 2.3 BIOS kurulumu](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#BIOS) <br/>
[* 3.Ubuntu 24.04'ü Yükleme](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#InstallUbuntu) <br/>
[  ** 3.1 Dil seçimi](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#LangSec) <br/>
[** 3.2 Sistem yükleyicisini yükleme](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#Loader) <br/>
[** 3.3 Dil seçimi](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#LanguageAgain) <br/>
[** 3.4 Klavye Düzeni](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#Layout) <br/>
[** 3.5 Yazılım](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#Software) <br/>
[** 3.6 Disk nasıl bölümlenir](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#PartDist) <br/>
[** 3.7 Yeni Bölüm Tablosu](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#PartTable) <br/>
[** 3.8 Önyükleyici bölümü oluşturma](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#BootLoad) <br/>
[** 3.9 Kök bölümü oluşturma](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#RootPart) <br/>
[** 3.10 Ev bölümü oluşturma](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#HomePart) <br/>
[** 3.11 Disk bölümlendirmeyi tamamlama](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#FinPart) <br/>
[** 3.12 Zaman Dilimi](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#TZ) <br/>
[** 3.13 Kullanıcı oluşturma](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#CreateUser) <br/>
[** 3.14 Sistemin kurulumu](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#InstSys) <br/>
[** 3.15 Yeniden Başlatma](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#Reboot) <br/>
[* 4. Sonuçlar](https://github.com/MusubaPy/Install-Ubuntu-guide?tab=readme-ov-file#Conclusion) <br/>
## 1. Ubuntu sistem gereksinimleri
**Kuruluma başlamadan önce aşağıdakileri göz önünde bulundurmanız gerekir:** <br/>

  **Dizüstü bilgisayarınızı bir güç kaynağına bağlayın.* <br/>
  **En az 25 GB boş depolama alanınız olduğundan emin olun veya minimum kurulum için 5 GB boş depolama alanınız olsun.* <br/>
  **Yüklemek istediğiniz Ubuntu sürümünü içeren bir DVD'ye veya USB flash sürücüye erişiminiz olsun.* <br/>
  **Verilerinizin yakın zamanda yedeğini aldığınızdan emin olun. Herhangi bir şeyin ters gitmesi pek olası olmasa da, asla fazla hazırlıklı olamazsınız.* <br/>
  
**Minimum sistem gereksinimleri:** <br/>

  **2 GHz çift çekirdekli işlemci* <br/>
  **4 GiB RAM (sistem belleği)* <br/>
  **50 GB (en az 8,6 GB) sabit disk alanı (veya USB bellek, hafıza kartı veya harici sürücü, ancak alternatif bir yaklaşım için LiveCD'ye bakın)* <br/>
  **1024x768 ekran çözünürlüğüne uygun VGA* <br/>
  **Kurulum ortamı için bir CD/DVD sürücüsü veya bir USB bağlantı noktası* <br/>
  **İnternet erişimi faydalıdır* <br/>
  
## 2. Ubuntu'yu yüklemeye hazırlanıyor 

*Sistemi kurmaya başlamadan önce her şeyi hazırlamamız gerekiyor. İlk yapmamız gereken şey resmi siteden kurulum imajını indirmek.* <br/>

**2.1 Görüntünün indirilmesi** <br/>

*Ubuntu web sitesini açın ve Masaüstü sürüm görüntüsünü indirin.* <br/>

![Ekran görüntüsü 2024-10-26 182736](https://github.com/user-attachments/assets/e9733a3b-10dc-4938-9a2c-2cc7dc148875) <br/>

**2.2 Görüntüyü bir USB belleğe yazma** <br/>

*Görüntü indirildikten sonra, bir kurulum ortamına - bir flash sürücüye - yazdırılması gerekir. Etcher yardımcı programını veya Unetbootin'i kullanarak onu bir Linux flash sürücüsüne yazabilirsiniz. Windows'ta bir flash sürücüye yazmak için Rufus yardımcı programını kullanabilirsiniz .* <br/>

**2.3 BIOS kurulumu** <br/>

*Çoğu bilgisayar USB'den otomatik olarak önyükleme yapacaktır. USB flash sürücüyü takın ve bilgisayarınızı açın veya yeniden başlatın. Dilinizi seçmenizi ve Ubuntu masaüstünü yüklemenizi veya denemenizi isteyen bir karşılama penceresi görmelisiniz.* <br/>

*Bilgisayarınız USB'den otomatik olarak önyükleme yapmıyorsa, bilgisayarınız ilk başladığında F12'yi basılı tutmayı deneyin . Çoğu makinede bu, USB aygıtını sisteme özgü bir önyükleme menüsünden seçmenize olanak tanır.* <br/>

**F12, sisteminizin önyükleme menüsünü açmak için en yaygın tuştur, ancak Escape , F2 ve F10 yaygın alternatiflerdir. Emin değilseniz, sisteminiz başladığında kısa bir mesaj arayın - bu genellikle önyükleme menüsünü açmak için hangi tuşa basmanız gerektiği konusunda sizi bilgilendirir.* <br/>

*Otomatik önyükleme başlamazsa, bilgisayarı sabit sürücünüzden değil, yeni kaydedilmiş bir USB yükleyicisinden önyükleme yapacak şekilde ayarlamanız gerekir. Bunu yapmak için, bilgisayarınızı yeniden başlatın ve BIOS açılış ekranı sırasında Del , F8 , Shift+F2 veya başka bir tuş kombinasyonuna basarak BIOS kurulum menüsünü açın.* <br/>

![175530047-57618fd6-1c2e-4082-bd1c-1677226222b8](https://github.com/user-attachments/assets/aea329ec-6311-4c81-b89e-5dee5e08c045)

*Burada Boot sekmesine gitmeniz ve ardından Boot device priority bölümünde flash sürücünüzü veya DVD'nizi ilk sıraya ayarlamanız gerekir. Ardından sadece Exit sekmesine gitmeniz ve Exit & Save settings'e tıklamanız gerekir .* <br/>

*Daha fazla bilgi için web sitesine gidin .* <br/>

**3.Ubuntu 24.04'ü Yükleme** <br/>

*Daha sonra bilgisayarınızı yeniden başlatmanız gerekiyor ve doğrudan işletim sistemini yüklemeye geçeceğiz.* <br/>

**3.1 Dil seçimi** <br/>

*Yeniden başlatmanın hemen ardından şu pencereyi göreceksiniz:* <br/>

![Ekran görüntüsü 2024-10-26 144654](https://github.com/user-attachments/assets/3004f9d9-b783-405b-9b75-6b01b447210b)

*Bu adımı atlayıp Ubuntu kurulumunun hemen İngilizce olarak başlamasını sağlayabilirsiniz ancak herhangi bir tuşa basıp İngilizce seçeneğini seçmeniz daha iyi olacaktır.* <br/>

**3.2 Sistem yükleyicisini yükleme** <br/>

*Açılan menüde Ubuntu'yu Kur seçeneğini seçin , kurulum başlayacaktır.* <br/>

![175869770-c0022d28-4063-413f-86c1-6329e18c11be](https://github.com/user-attachments/assets/4695309a-52e2-4869-b56e-dfef3d166071)

**3.3 Dil seçimi** <br/>

*Varsayılan olarak sistem İngilizce'yi seçecektir. Siz İngilizce'yi seçmelisiniz .* <br/>

*Gelecekteki sisteminiz için bir dil seçin:* <br/>

![Ekran görüntüsü 2024-10-26 144654](https://github.com/user-attachments/assets/944dea67-dce2-4b81-8b60-e3c214a1793a)

**3.4 Klavye Düzeni** <br/>

*Varsayılan klavye düzenini seçin. Kurulum sırasında düzeni değiştirmeniz gerekirse bunu Alt+Shift veya Win+Space ile yapabilirsiniz .* <br/>

*Varsayılan olarak sistem İngilizce'yi seçecektir. Siz İngilizce'yi seçmelisiniz .* <br/>

*Standart olmayan bir klavyeniz varsa, listeden seçebilirsiniz. Alternatif olarak, Klavye Düzenini Algıla'ya tıklayın ve sistem otomatik olarak klavyenizi seçecektir. Klavyenizi test etmeniz gerekiyorsa, etiketli alanı kullanın.* <br/>

*Hazır olduğunuzda Devam'a tıklayın .* <br/>

![Ekran görüntüsü 2024-10-26 185525](https://github.com/user-attachments/assets/39f7aa2f-b0cb-42ae-8a8f-a3000b3719e8)

**3.5 Yazılım** <br/>

*Başlangıçta hangi uygulamaları yüklemek istediğiniz sorulacak. İki seçenek 'Normal kurulum' ve 'Minimal kurulum'dur. İlki, eski varsayılan yardımcı program, uygulama, oyun ve medya oynatıcı paketine eşdeğerdir — herhangi bir Linux kurulumu için harika bir başlatma rampası. İkincisi önemli ölçüde daha az depolama alanı kaplar ve yalnızca ihtiyacınız olanı yüklemenize olanak tanır.* <br/>

*Kurulum türü sorusunun altında iki onay kutusu bulunur; biri kurulum sırasında güncellemeleri etkinleştirmek, diğeri ise üçüncü taraf yazılımları etkinleştirmek içindir.* <br/>

**Hem Güncellemeleri indir hem de Üçüncü taraf yazılımları yükle seçeneklerinin ikisini de etkinleştirmenizi öneririz .* <br/>
**Ubuntu'yu kurarken en son güncellemeleri alabilmeniz için internete bağlı kalın.* <br/>
**İnternete bağlı değilseniz, varsa kablosuz bir ağ seçmeniz istenecektir. Makinenizin güncel olduğundan emin olabilmemiz için kurulum sırasında bağlanmanızı öneririz.* <br/>

![Ekran görüntüsü 2024-10-26 185546](https://github.com/user-attachments/assets/ebfae1c5-bb12-4077-b581-2d07ac15746a)

**3.6 Disk nasıl bölümlenir** <br/>

*Ubuntu'yu başka bir işletim sistemiyle birlikte kurmak, mevcut işletim sisteminizi silmek ve yerine Ubuntu kurmak isteyip istemediğinizi seçmek için onay kutularını kullanın.* <br/>

**Windows zaten yüklüyse, yükleyicinin bölümlendirmeyi otomatik olarak yapmasına güvenebilirsiniz. Install Ubuntu alongside Windows Boot Manager'ı seçin .* <br/>
**Ubuntu'yu kurmadan önce Diski sil ve Ubuntu'yu kur seçeneğine tıklayarak sabit sürücüyü temizleyebilirsiniz .* <br/>
**Something else seçeneğini seçin . Bunu kendi disk bölümlerinizi belirtmek veya diğer gelişmiş seçenekleri ayarlamak için kullanın.* <br/>

![Ekran görüntüsü 2024-10-26 185632](https://github.com/user-attachments/assets/6b4d1027-81ea-4c74-8b36-8b62a4bc9b41)

*Yan yana kurulum veya önceki bir kurulumu silmeyle ilgili seçenekler yalnızca önceden var olan kurulumlar algılandığında sunulur.* <br/>

**3.7 Yeni Bölüm Tablosu** <br/>

*Tüm boş alanı root'a ayırmayı seçebilirsiniz (swapfile ve home otomatik olarak root altında oluşturulacaktır) veya root, swap ve home bölümlendirmesini ayırabilirsiniz. Her iki yöntem de iyidir.* <br/>

*Root, / ve home bölümlerini ayrı ayrı oluşturma adımlarını gösteriyorum. Ancak hepsi için tek bir bölüm kullanmaktan çekinmeyin.* <br/>

![Ekran görüntüsü 2024-10-26 191743](https://github.com/user-attachments/assets/e55e8016-4bb3-400d-86d4-7a3b17787b3d)

*Geleneksel olarak Linux'ta üç bölüm oluşturulması önerilir:* <br/>

**/ boot önyükleyici için;* <br/>
**/ işletim sisteminin kendisi için;* <br/>
**/home kullanıcı dosyaları için.* <br/>

*Bu şemayı takip edeceğiz. Prensip olarak, /boot bölümünü oluşturmanız gerekmez , ancak birden fazla Linux dağıtımı kuracaksanız tavsiye edilir.* <br/>

**3.8 Önyükleyici bölümü oluşturma** <br/>

*Bir bölüm oluşturmak için, Boş alanı seçin ve + (artı) işaretine tıklayın. Size bir Linux bölümü oluşturma seçeneği sunacaktır. Açılan pencerede bölümün boyutunu seçmeniz gerekecektir. Son zamanlarda önyükleyici çok fazla yer kaplıyor, bu yüzden en azından 300 megabayt bırakmak daha iyidir.* <br/>

*Boyutu seçin, dosya türü olarak Ext2'yi ve bağlama noktası olarak /boot'u seçin.* <br/>

*Daha sonra "Tamam" butonuna tıklayın .* <br/>

**3.9 Kök bölümü oluşturma** <br/>

*Root bölümünü oluşturuyorsunuz. 50 GB'ın üzerindeki her şey bunun için fazlasıyla yeterlidir. Boyutu seçin, dosya türü olarak Ext4'ü ve bağlama noktası olarak / (root anlamına gelir) seçin.* <br/>

*/boot ve /home bölümleri atlanabilirse , bu bölüm zorunludur. İşletim sistemi burada bulunacaktır. /boot ve /home bölümlerini oluşturmazsanız , dosyaları da bu bölümde olacaktır.* <br/>

![Ekran görüntüsü 2024-10-26 192532](https://github.com/user-attachments/assets/500b773b-9b5d-4b45-8376-ce5e3bc04328)

**3.10 Ev bölümü oluşturma** <br/>

*Benzer şekilde, bir Ev bölümü oluşturun. Buraya maksimum alanı ayırın (aslında kalan boş alanı ayırın) çünkü müzikleri, resimleri ve indirilen dosyaları buraya kaydedeceksiniz.* <br/>

![Ekran görüntüsü 2024-10-26 192503](https://github.com/user-attachments/assets/ebc172e5-b68e-4dc0-a685-a8d3c4db2f7c)

**3.11 Disk bölümlendirmeyi tamamlama** <br/>

*Boot, Root ve Home'a ​​hazır olduğunuzda Şimdi Yükle'ye tıklayın :* <br/>

![Ekran görüntüsü 2024-10-26 192624](https://github.com/user-attachments/assets/91eac80f-c36c-4846-92e1-55360d313996)

*>>>>PS Bu görsel sizinkinden farklı olabilir.<<<<* <br/>

**3.12 Zaman Dilimi** <br/>

*İnternete bağlıysanız konumunuz otomatik olarak algılanacaktır. Konumunuzun doğru olduğundan emin olun ve devam etmek için 'İleri'ye tıklayın.* <br/>

*Saat diliminizden emin değilseniz, yerel bir kasaba veya şehrin adını yazın veya konumunuzu seçmek için haritayı kullanın.* <br/>

![Ekran görüntüsü 2024-10-26 185708](https://github.com/user-attachments/assets/2c8f4d04-ff03-4943-b7d3-a7e2d155bdbf)

*>>>>PS İnternete bağlanmada sorun yaşıyorsanız, sağ üst köşedeki menüyü kullanarak bir ağ seçin.<<<<* <br/>

**3.13 Kullanıcı oluşturma** <br/>

*Adınızı girin ve yükleyici otomatik olarak bir bilgisayar adı ve kullanıcı adı önerecektir. İsterseniz bunlar kolayca değiştirilebilir. Bilgisayar adı, bilgisayarınızın ağda nasıl görüneceğidir, kullanıcı adınız ise oturum açma ve hesap adınız olacaktır.* <br/>

*Sonra bir parola girin. Yükleyici çok zayıfsa size bildirecektir.* <br/>

![Ekran görüntüsü 2024-10-26 185653](https://github.com/user-attachments/assets/8c294332-27a1-4cce-a66f-af4ced1782fa)

**3.14 Sistemin kurulumu** <br/>

*Kurulum penceresi size Ubuntu'nun ne kadar harika olduğunu biraz öğretirken yükleyici artık arka planda tamamlanacaktır. Makinenizin hızına ve ağ bağlantınıza bağlı olarak, kurulum yalnızca birkaç dakika sürecektir.* <br/>

![Ekran görüntüsü 2024-10-26 193328](https://github.com/user-attachments/assets/83911e69-f5a7-4257-9b9b-b674d882ce15)

**3.15 Yeniden Başlatma** <br/>

*Her şey yüklendikten ve yapılandırıldıktan sonra, makinenizi yeniden başlatmanızı isteyen küçük bir pencere açılacaktır. Şimdi Yeniden Başlat'a tıklayın ve istendiğinde DVD veya USB flash sürücüyü çıkarın.* <br/>

![Ekran görüntüsü 2024-10-26 194747](https://github.com/user-attachments/assets/95f9ed0e-a637-444b-b28e-00d4b51fbaf7)

**4. Sonuçlar** <br/>

*Tebrikler! Dünyanın en popüler Linux işletim sistemini başarıyla kurdunuz!* <br/>

*Artık Ubuntu'nun tadını çıkarmanın zamanı geldi!* <br/>

*Ubuntu'nun diğer sürümleri de aynı şekilde kurulur.* <br/>
