## 1) HTML Nedir?

- Html aslında bir işaretleme dilidir.
- 1980'lerin başında ilk çıkmıştır, 1989'da tam anlamıyla kullanılmaya başlanmıştır.
- Bu etiketleme dilinde daha sonra CSS eklenir ve anlamlı görünümler elde ederiz.
- WEB Sitemizin iskeletini aslında HTML ile oluştururuz
- HTML bir programa dili değildir.

## 2) En Çok Kullanılan HTML Etiketleri Nelerdir

- Etiketten kasıt aynı türden başlayı aynı türden bitirmektir.
- "/" etiketin kapandığını belirtmek gerekir.
- Bir web sitesinde aşağıdaki şeylere ihtiyacımız olabilir.
- **Başlık**: H1 ile başlar ve H2, H3, H4, H5, H6 olarak ilerler.
- Paragraf
    - Link
    - Resim / Görsel
    - Listeler (Sıralı/Sırasız(Bullet))
    - Tablo
    - Form
- HTML içerisinde 200'den fazla etiket olsa da biz genelde yaklaşık 15 adet kullanıyoruz.
- **Not:** Bazı etiketler kapanmaya ihtiyaç duymazlar. Örneğin: `<br>, <hr>, <meta>`
- Eğer bir HTML dökümanı oluşturmak isterseniz ilk yapacağınız iş bir `<html>` etiketi eklemektir. Ve içerisinde `<body>` etiketi barındırmalıdır.
- **HEAD Etiketi:**
    - `<head>` etiketi, site ziyaretçileri tarafından görülmesi gerekmeyen kodları içerir. Bu etiket altına yazılan kodlar genellikle arama motorları ve örümcekler (Crawler veya Spider diye geçer) içindir. Head etiketi altında bütün etiketleri kullanabilmeniz mümkün değil. Kullanabileceğiniz etiketler;
        - `<title>` (Bu etiketi kullanmak şarttır)
        - `<meta>`
        - `<style>`
        - `<script>`
        - `<noscript>`
        - `<link>`
        - `<base>`

- **BODY etiketi:** Web sayfamızda görmek istediğimiz etiketleri buraya yazarız.
- **H `<h1,2,3,4,5,6>`** etiketleri başlıklar, **P `<p>`** etiketi paragraflar içindir
- **Not:** HTML otomatik olarak paragraf etiketinin öncesine ve sonrasına satır atlatır.
- **BR Etiketi:** `<br>` etiketi satır atlama etiketidir. Kapatma ihtiyaç duymayan etiketlerden biridir. Atlatmak istediğiniz satır sayısı kadar `<br>` etiketi kullanabilirsiniz.
- **NOT:** BR etiketinin farklı kullanımlarını görebilirsiniz. *örn.*(`<br>`,`<br/>`,`<br />`) Hepsi aynı işlevi yerine getirir.
- **********************A Etiketi: `<a>`** etiketinin en önemli özelliği **href** özelliğidir. Bu etiket ile sayfaları linkleyebiliriz. Etiket içerisine yazılan içerik sayfa üzerinde gösterilecek içeriktir. href içine yazılan ise tıklandığında gideceği URL'dir.
- **UL - OL - Li Etiketi:**
    
    `<ul>` ve `<ol>` etiketleri liste oluşturma etiketleridir. Listeyi oluşturduktan sonra içeriğini oluşturmak için `<li>`etiketini kullanıyoruz.
    
    `<ul>` = **"unordered list"** sırasız liste anlamına geliyor. `<ol>` = **"ordered list"** sıralı liste anlamına geliyor.
    
- **Strong ve B etiketi:** `<strong>` etiketi bir metinin arama motorlarına önemli olduğunu bildirmek için kullanılır. Kullanıldığı zaman metini kalın yapar. Eğer sadece metini kalınlaştırmak isterseniz `<b>` etiketini kullanabilirsiniz.
- Script Etiketi: `<script>` etiketi JavaScript kodlarını HTML içerisine yazabilmemizi sağlar.
- **Button Etiketi:** `<button>` etiketini buton oluşturmak için kullanırız. Buton üzerine yazmak istediğiniz içeriği etiketin içine yazmanız yeterlidir.
- **img Etiketi:** Resim eklemek için`<img>` etiketini kullanıyoruz. `<img src=”resim.jpg” alt=”açıklama yazısı” />` **src=""**kısmına eklemek istediğimiz görselin yolunu yani kaynağını yazmalıyız. Eğer görselimiz ve HTML dosyamız aynı klasörde ise görselin adını ve uzantısını yazmamız yeterlidir. **alt=""** kısmına görselin açıklamasını yazıyoruz fakat isterseniz boş bırakabilirsiniz. Bu etiket kapanmaya ihtiyaç duymaz.
- **iframe Etiketi:** Belge içinde belge gösterebilmemizi sağlayan etikettir. Genelde başka bir sitedeki belgeyi kendi sayfamızda göstermek için kullanırız. *örn:* Youtube'dan bir videoyu sayfamızda göstermek istersek `<iframe>` kodlarını sayfamıza eklememiz yeterli.(video üzerinde sağ tıklayıp yerleştirme kodunu kopyala diyerek iframe kodunu kopyalayabiliriz.)
- **Yorum Satırı:** HTML dilinde yorum satırı`<!--` ile başlar `-->` ile biter.
- Tüm anlatımların kod örneği:
    
    ```html
    <!DOCTYPE html>
    <html lang="tr">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>En çok kullanılan html etiketleri</title>
    </head>
    <body>
        <!-- Örnek Yorum Satırı -->
        
        <!-- 
            2. Örnek Yorum Satırı 
        -->
    <h2><strong> Kodluyoruz </strong></h2>
    <p><b> HTML </b> Etiketleri </p>
    <hr/>
    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
     </ul>
    
      <hr>
        
    <ol>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
    </ol>
     
    <button> Buton </button>
    <br/>
    <a href="https://www.kodluyoruz.org">
       <img src="https://cdn.sanity.io/images/9kdepi1d/production/65c832d202a503b15d99e628f4313782f3ef50db-300x62.png" alt=”Kodluyoruz Bootcamp” />
     </a>
    
    <br/>
    <iframe width="100" height="100"   src="https://www.youtube.com/embed/BHPYQHnD_QA" frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
    </iframe>
    </body>
    </html>
    ```
    

## 3) Başlık Etiketleri Kullanımı

- Bu noktada `<head></head>` etiketi arasına yazılan etiketlerden bahsedeceğiz.
- **Title Etiketi:**
    - Bu etiketimiz html dökümanlarında türkçe anlamı olan "başlık" görevini üstlenir. Bu başlık birkaç farklı yerde görülebilir. Bizim en sık karşılaştığımız şekli ise browser sekmelerinin isimleridir. Örnek olarak :
        
        ```
        <title> Kodluyoruzla Web Öğreniyorum </title>
        ```
        
        Gibi bir başlık belirlediğimizde sekme isminde Kodluyoruzla Web Öğreniyorum yazdığını görürüz.
        
        Bu etiket arasına yazdıklarımız aynı zamanda sayfayı favorilere eklerken de karşımıza çıkar.
        
        Ayrıca arama motorları (Google, Yahoo, Bing ...) sayfamızın bu kısmına bakarak sitemizi listeler. Bu yüzden de oluşturduğumuz mükemmel web sayfalarının insanlara ulaşması için bu alanda yazdıklarımızın açıklayıcı, dikkat çekici ve 50-60 karakteri geçmeyecek şekilde ( Arama motorları genelde başlığın ilk 50-60 karakterini gösterir ) yazmamız gerekir.
        
- **Style ve Script Etiketleri:**
    - HTML dökümanları oluştururken en çok kullanacağımız etiketler bunlardır. Bu etiketler yalnızca `<head></head>`etiketleri arasında bulunmaz ancak biz burada bulunabilecek bazı özel türleri ve bu tür etiketlerin özelliklerini (attribute) inceleyeceğiz.
    - Öncelikle style etiketinden başlayalım. `<style></style>` etiketleri arasında sayfamızı güzelleştiren, renklendiren belli özellikler tanımlayabiliyoruz. Bu kısımlarda, bir html dökümanında hangi alanın nerede ve nasıl görünmesi gerektiğini tasarlayabiliriz. Belli kuralları olan bu belirteçlere CSS diyoruz. Sayfa tasarımlarının bulunduğu bir ön döküman veya bir taslak gibi düşünebiliriz. CSS ile daha detaylı bilgi için şurayı inceleyebilirsiniz : https://www.w3schools.com/css/default.asp
    - Burada dikkat etmemiz gereken bir konu var. HTML dökümanı işlenirken ve görüntülenirken sayfa sırayla işlendiği için her zaman sırasıyla en altta kalan stil belirlemeleri baskın gelecektir.
    - Bu etiketimizin global özelliklere(attribute) ek olarak alabildiği iki farklı özellik vardır. Bunlar media ve type. Çok yaygın olmadığı için kullanım detaylarına girmeyeceğim ama alabildikleri özelliklere şuralardan bakabilirsiniz :https://www.w3schools.com/tags/att_style_media.asp
    - Geldik web dökümanlarının ön yüzlerini "sihirli" hale getiren etikete. Bu etiketle web sayfalarının, browser yardımıyla çalıştırabildiği kodlar yazabiliriz. Sayfamızı canlandırabilir, hareketlendirebilir her alanda değişiklik yapabiliriz. Sayfamız üzerinde hayal gücümüzle sınırlı her değişikliği yapabilmemizi sağlayan kodlar bu etiketler arasında bulunur.
    - `<script></script>` etiketleri ileride öğreneceğiniz sihirli bir dünyaya açılan kapıdır. Normalde HTML dökümanlarının bir programlama dili ile yazılmadığını biliyoruz. Çünkü HTML ve CSS bir programlama dili değildir. Ancak`<script></script>` tagları arasına girdiğimizde işler değişmeye başlıyor. Artık bir programlama dili olan JavaScript'in dünyasına girmiş oluyoruz. HTML dökümanlarının stilleri yerleşimleri hatta bütün dökümanın kendisini Javascript yardımıyla değiştirebilir, farklı işlemler yapabilir, farklı sayfalarla veya arka planda bir veri tabanıyla haberleşebilir oradan aldığımız bilgilerle dökümanımızı güncelleyebiliriz. Ayrıca HTML dökümanımıza yeni elemanlar ekleyip çıkartabiliriz. Dökümanlarımız üzerinde hareketli animasyonlar çalıştırabilir, her türlü değişikliği yapabiliriz. Bu yüzden bu etiketlerin bizim gücümüzü artıran sihirli bir dünyaya açıldığını söyleyebiliriz. Şimdi bunun özelliklerine bakalım.
- **Script Tag Özellikleri:**
    
    Öncelikle bu etiketlerin bize sayfa üzerinde büyük bir güç verdiğinden bahsetmiştik. Ancak Spider Man Peter Parker'ın rahmetli amcasının da dediği gibi "with great power comes great responsibility" yani büyük güç büyük sorumluluk gerektirir. Bu yüzden bu tagın özelliklerinden bahsederken sayfanın işlenişi, browser tarafında nasıl işlendiğini ve yanlış bir kullanımın nelere sebep olabileceğini iyi anlamamız gerekiyor. Eğer script etiketini kullanırken herhangi bir özellik eklemezsek browser sırası geldiğinde doğrudan işlenir. Ve bu kısım işlenmeden sayfa yüklenmeye devam etmez. Bu noktada da *async* özelliğimiz devreye giriyor. Eğer sayfanın yüklenmeye devam ederken eşzamanlı olarak bu etiketlerle belirlediğimiz scriptlerin de yüklenmesini ve hazırlanmasını istiyorsak, yani bu kısmın asenkron çalışmasını istiyorsak etiketimize bu özelliği ekliyoruz. Herhangi bir değer girmemize gerek yok şu şekilde kullanabiliriz :
    
    ```
    <script src="myJavascript.js" async></script>
    ```
    
    Eğer bu etiketin sayfa yüklendikten sonra yüklenip çalıştırılmasını istiyorsak o zaman async özelliğinin yanına *defer*özelliğini de eklememiz gerekiyor. Ancak bu iki özellik de yalnızca sayfa harici kaynaktan yani bu HTML içinde yazmadığımız javascripti yüklerken kullanabileceğimiz özellikler. Buna da dikkat etmemiz gerekiyor.
    
    Bu etiketin sihirli dünyasından bahsetmiştik. Ancak bahsetmediğimiz nokta her sihirli dünyada olduğu gibi burada da kötü büyücülerin, kötü insanların olduğudur. Bu yüzden sayfamız üzerinde bu kadar güce sahip bir alanın doğru şekilde korunması ve kullanılması hayati önem taşıyor. İşte bu amaçla da karşımıza iki özellik çıkıyor.
    
    Bu özelliklerden birincisi crossorigin. Browserlar, istek sahteciliği gibi güvenlik sorunlarıyla aktif şekilde mücadele etmeye çalışıyor. Bu yüzden bir kaynaktaki dökümanın bir diğer kaynaktaki (farklı domain) dökümanlara erişmesinde biraz hassas davranıyorlar. Bu konuya cross origin resource sharing deniyor kısaca CORS diyebiliriz. İşte bu etiketimiz de farklı kaynaklardaki, farklı domainlerdeki scriptleri yüklememiz için bize yardımcı oluyor. Eğer bir kaynaktan(aynı domain dahil) bir şey yüklemek için belli bilgileri( Çerezlerimiz olabilir, HTTP basit giriş bilgileri olabilir) göndermemiz gerekiyorsa bu özelliğin değerini crossorigin = "use-credentials" olarak belirlemeliyiz. Eğer anonim şekilde erişmemiz gerekiyorsa yani herhangi bir bilgiye ihtiyaç yoksa crossorigin="anonymous" olarak kullanacağız.
    
    Bir diğer özelliğimiz ise integrity özelliğidir. Integrity türkçeye bütünlük, doğruluk, dürüstlük şeklinde çevirilebilir. Webin gelişmesiyle birlikte bir HTML sayfasına yüklenen kaynaklar çoğaldı. Özellikle tekrar eden ihtiyaçlar için zaman geçtikçe en verimli çözümler üretilmeye ve kullanılmaya başlandı. Bu çözümlerin kullanılması yaygınlaştıkça belli riskler de ortaya çıkmaya başladı. Örnek olarak HTML sayfamıza ekleyeceğimiz bir dış script bir güvenlik açığıyla karşı karşıya kaldığında o scripti kullanan bütün sayfalar aynı anda etkilenmiş olacak. Bunun bir örneği yakın zamanda birçok firmayı etkileyen Gigya servisinde olmuştu. Bu servisi kullanan sitelerin sayfalarına ekledikleri harici bir gigya servisi bir saldırıya maruz kalmıştı ve o servisi kullanan binlerce sitede bu açıktan etkilenmişti. İşte CDN dediğimiz bu gibi hazır scriptleri eklediğimiz durumlarda bir doğrulama yöntemine ihtiyaç duyuyoruz. Yani browser bir şekilde, sayfamızı etkileyecek kodların bizim istediğimiz eklediğimiz kodlar olduğunu doğrulaması gerekiyor. Bu noktada da integrity özelliği devreye giriyor. Sayfamızda kullanacağımız hazır kodların bir imzasını bu özelliğe değer olarak ekliyoruz. Bu imza doğrudan kodun kendisinden oluşturulur ve belli bir karakter uzunluğundadır. Ayrıca kodda bir harf bile değişecek olsa imza tutmayacaktır. Bu sayede eğer kodda zararlı/zararsız herhangi bir değişiklik olursa browser imzalar uyuşmayacağı için kodları sayfamıza yüklemeyecektir.
    
    **Örnek olarak şu şekilde kullanabiliriz :**
    
    ```
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js" integrity="sha384-0mSbJDEHialfmuBBQP6A4Qrprq5OVfW37PRR3j5ELqxss1yVqOtnepnHVP9aJ7xS" crossorigin="anonymous"></script>
    ```
    
    Bir diğer etiketimiz de refreferrerpolicy. Bu etiket de scripti yükleyeceğimiz zaman, alacağımız kaynağa atacağımız verileri eklemek için kullınılır. Detaylı kullanımına buradan bakabilirsiniz :https://www.w3schools.com/tags/att_script_referrepolicy.asp Bu da crossorigin gibi kaynak paylaşımı maksadıyla kullanılan özelliklerdendir.
    
    HTML sayfamızı oluştururken sayfa içerisindeki kod ne kadar uzun olursa okunması, yazılması ve incelenmesi o kadar zor olur. Bu yüzden kodları farklı sayfalara bölüp kullanmak hem daha kullanışlı hem de daha verimli olur. İşte bu amaçla farklı sayfalardaki scriptleri yükleyebilmek için de script etiketini kullanabiliriz. Bu amaçla script etiketinin *src*özelliğini kullanırız. Bu özellikle hem kendi dosya sistemimizde hem de internet üzerinde herhangi bir adreste bulunan kodları kendi sayfamıza ekleyebiliriz.
    
    Örnek olarak kendi dosya sistemimizde, html dökümanımızla aynı dizinde bulunan bir script dosyasını çağırmak için:
    
    ```
    <script src="myJavascript.js"></script>
    ```
    
    Veya bir web sayfasındaki başka bir scripti çağırmak için :
    
    ```
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js" integrity="sha384-0mSbJDEHialfmuBBQP6A4Qrprq5OVfW37PRR3j5ELqxss1yVqOtnepnHVP9aJ7xS" crossorigin="anonymous"></script>
    ```
    
    Son olarak da bu etiketle kullanabileceğimiz type özelliğimiz, yüklenecek dosyanın içeriğinin, browser tarafından nasıl yorumlanması gerektiğini belirtir. Örnek olarak javascript dosyası yüklemek için yüklenecek kodların javascript kodunu belirtmek için şöyle yazabiliriz :
    
    ```
    <script type="application/javascript">document.getElementById("someTestDiv").innerHTML = "This code runs as js";
    </script>
    
    ```
    
    Ya da Ecmascript için :
    
    ```
    <script type="application/ecmascript">document.getElementById("someTestDiv").innerHTML = "This code runs as js";
    </script>
    ```
    
- **Link Etiketi:**
    
    Script etiketini anlatırken bir HTML dökümanında yüklenecek kodların bölünmesinin bir çok kolaylık sağlayacağından bahsetmiştik. İşte `<link></link>` etiketi de script etiketinin src özelliği ile kullanılması gibi link etiketini de farklı kaynaklardan farklı dosyaları HTML dökümanımıza dahil etmek için kullanabiliriz. Bu etiket dökümanımızda bulunmayan dış kaynaklarla dökümanımız arasındaki ilişki kurmak için kullanılır.
    
    Bu etikette de crossorigin özelliği mevcuttur.
    
    Bu etikette ilişki kurmak istediğimiz dış kaynağı href özelliği ile veriyoruz. Bu özelliğin açılımı Hypertext REFerence şeklindedir. Örnek olarak bir CSS sayfasını HTML dökümanımız ile ilişkilendirmek için şu kodu kullanabiliriz :
    
    ```
    <link rel="stylesheet" href="styles.css">
    ```
    
    href özelliğini hem dış kaynaklardan hem de dökümanımızın bulunduğu dosyadan ilişkilendirme yapmak için kullanabiliriz.
    
    ```
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z" crossorigin="anonymous">
    ```
    
    Bu etiketin önemli özelliklerinden birisi de *rel* özelliğidir. Bu özellik dış kaynaktaki dosyayı kendi HTML dökümanımıza ne şekilde ilişkilendirmek istediğimizi belirttiğimiz kısımdır. En çok kullanılan değerleri "stylesheet" ve "icon" dur. Stylesheet eklemek istediğimiz dosyanın bir stil dosyası olduğunu söyler. Böylece browser oradaki komutları HTML'imizi şekillendirmede ve değiştirmede kullanır.
    
    Yukarıda HTML dökümanımızın stil ve script dosyalarını ayrı ayrı yazmanın faydalarından bahsetmiştik. Script etiketi ile bu javascript dosyalarını ekleyebiliyorduk ancak CSS yani stil dosyalarını eklemenin yöntemini öğrenmemiştik. İşte bu link etiketi ve rel özelliği yardımıyla istediğimiz stil dosyasını da `<head></head>` etiketlerinin arasında ekleyerek web sayfamızı daha renkli ve eğlenceli hale getirebiliriz.
    
    `<title></title>` etiketi yardımıyla sekmelerde görünecek, HTML dökümanımızın başlık ismini belirlemiştik. Ancak şu an bu yazının olduğu sekmeye bakarsanız başlığın yanında bir de küçük bir logo/ikon göreceksiniz. İşte bu ikonlar eklemek için de rel = "icon" kullanıyoruz. Bulunduğumuz dizinde **.ico** uzantılı bir **favicon.ico** dosyamız varsa bu dosyayı sekmelerde ismin yanında ikon olarak göstermek üzere şöyle bir kod kullanabiliriz :
    
    ```
    <link rel="icon" href="/favicon.ico" type="image/x-icon">
    ```
    
    Son olarak link etiketi de type özelliği kullanır. Bu özellikle de ilişkilendirdiğimiz dosyanın tipini vermiş oluyoruz. Yaygın kullanılan değerleri stil dosyaları için `type = "text/css"` şeklinde, ikonlar için de `type="image/x-icon"`şeklindedir.
    
    Link etiketi global özellikleri de destekler. Diğer detaylı özellikleri için de buraya bakabilirsiniz : https://www.w3schools.com/tags/tag_link.asp
    
- **Meta Etiketi:**
    
    Tanıtacağımız son etiket ise meta etiketi. Meta veriler bilgisayar bilimleri dünyasında genellikle verinin verisi anlamında kullanılır. Yani bir veriyle ilgili bilgiler meta bilgiler olarak tanımlanır. İşte HTML dökümanımızla ilgili verilerin olduğu etiketler de meta etiketleridir. Burada vereceğimiz bilgiler sitemizi arama motorlarına, sosyal medyaya ve diğer sitelere tanıtmak ve dökümanımızla ilgili bilgiler vermek için kullanılacak veriler olacak.
    
    Sadece 4 farklı özelliği olan `<meta></meta>` etiketi dökümanımızla ilgili birçok bilgiyi barındıran farklı kullanım şekillerine sahip. Bu kullanımlar sayfamızla ilgili önemli bilgiler içerdiği için ayrı ayrı inceleyeceğiz.
    
    Dünyada farklı farklı diller ve farklı alfabeler mevcut. Örnek olarak latin alfabesi, arap alfabesi, çin alfabesi, elf alfabesi vs vs. Ancak hepsinde farklı karakterler olduğu için browserin bu karakterli görüntüleyebilmek için doğru şekilde çözümlemesi gerekir. İşte HTML dökümanımızdaki bu karakterlerin çözümlenme biçimlerini belirttiğimiz `<meta>`etiketi özelliğimiz *charset* özelliğidir. Bizim latin alfabesi için verilen charset kodu UTF-8 dir.
    
    ```
    <meta charset="UTF-8">
    ```
    
    Bir diğer önemli özelliğimiz ise http-equiv'dir. Browserlar farklı sunuculara istek atarlarken belli bilgileri karşı tarafa gönderirler. İşte bu isteklerin arasında isteğin detaylarıyla ve yöntemiyle ilgili bilgilerin olduğu header'lar bulunur. Biz de dökümanımızda o dökümana ulaşan birisinin browser'inde header alanında bir bilgi tutmak istiyorsak bu meta etiketi özelliğini kullanabiliriz. Örnek olarak charset ile belirttiğimiz özellik HTML5 ile gelmiştir. Daha önceki versiyonlarda ise şu şekilde bir kullanım vardır :
    
    ```
    <meta http-equiv="Content-type" content="text/html" charset="UTF-8">
    ```
    
    Ayrıca refresh başlığını(header) bu meta yardımıyla belirleyerek sayfamızın belli sürede bir yenilenmesini veya belli bir süre sonra başka bir sayfaya yönlendirilmesini sağlayabiliriz.
    
    ```
    <meta http-equiv="refresh" content="10;URL=kodluyoruz.html">
    ```
    
    Yukarıdaki kodda sayfa yüklendikten 10 saniye sonra URL ile verdiğimiz değer olan kodluyoruz.html'ye yönlendirilecek.
    
    Burada kullandığımız diğer etiket de *content* etiketidir. Bu da meta olarak verdiğimiz bilgilerin içeriğini tanımlamamızı sağlar.
    
    Son özelliğimiz de *name* özelliğimizdir. Bu da meta bilgi olarak vereceğimiz bilginin tanımlayıcısıdır diyebiliriz. Örnek olarak sayfamızda en çok geçen harfin ne olduğunu belirteceğimiz bir meta bilgisi yazmak isteyelim:
    
    ```
    <meta name="enCokGecenHarf" content="a">
    ```
    
    Bu şekilde istediğimiz meta bilgiyi sayfamızın başlık etiketleri arasında kullanabiliriz.
    
    Buraya kadar meta etiketini öğrendik peki sosyal medyalar ve arama motorları sitemizle ilgili bilgileri nasıl bu meta verilerden alıyor? Bu sorunun cevabı da yaygın kullanılan meta etiketleri kalıplarında bulunuyor. Örnek olarak github'da sağ tıklayıp sayfa kaynağını görüntüle dediğimizde karşımıza bir çok meta etiketi çıkıyor :
    
    ```
    <meta property="og:url" content="https://github.com"><meta property="og:site_name" content="GitHub">
    <meta property="og:title" content="Build software better, together">
    <meta property="og:description" content="GitHub is where people build software. More than 50 million people use GitHub to discover, fork, and contribute to over 100 million projects.">
    <meta property="og:image" content="https://github.githubassets.com/images/modules/open_graph/github-logo.png">
    <meta property="og:image:type" content="image/png">
    <meta property="og:image:width" content="1200">
    <meta property="og:image:height" content="1200">
    <meta property="og:image" content="https://github.githubassets.com/images/modules/open_graph/github-mark.png">
    <meta property="og:image:type" content="image/png">
    <meta property="og:image:width" content="1200">
    <meta property="og:image:height" content="620">
    <meta property="og:image" content="https://github.githubassets.com/images/modules/open_graph/github-octocat.png">
    <meta property="og:image:type" content="image/png">
    <meta property="og:image:width" content="1200">
    <meta property="og:image:height" content="620">
    
    <meta property="twitter:site" content="github">
    <meta property="twitter:creator" content="github">
    <meta property="twitter:card" content="summary_large_image">
    <meta property="twitter:title" content="GitHub">
    <meta property="twitter:description" content="GitHub is where people build software. More than 50 million people use GitHub to discover, fork, and contribute to over 100 million projects.">
    <meta property="twitter:image:src" content="https://github.githubassets.com/images/modules/open_graph/github-logo.png">
    <meta property="twitter:image:width" content="1200">
    <meta property="twitter:image:height" content="1200">
    
    ```
    
    İşte burada kullanılan meta taglar, facebook ve twitter paylaşımlarımızda bir url paylaşmak istediğimizde karşımıza çıkıyor. Sosyal medyada bir url paylaşmak istediğimizde url'yi kopyaladıktan sonra bir kart görürüz. Bu kartta bir başlık bir resim ve kısa bir açıklama bulunur. İşte o bilgiler bu meta verilerden alınır.
    
    Arama motorları bizi meta verilerinde verilen "keywords" lere göre sıralamaya alır :
    
    ```
    <meta name="keywords" content="Kodluyoruz,programlama,web">
    ```
    
    Ayrıca arama motorlarında sayfa başlığının altındaki açıklamalarda da yine bu meta verilerine öncelik verilir :
    
    ```
    <meta name="description" content="Kodluyoruzla web öğrenmeye hazır mısınız?">
    ```
    
    Bazı arama sonuçlarında yazar adı görürsünüz. Bu kısım da yine meta etiketinin marifetidir:
    
    ```
    <meta name="author" content="Kodluyoruz">
    ```
    
    Meta etiketiyle söyleyeceğimiz son şey de viewport konusu. Akıllı telefonlarla birlikte geliştiriciler artık farklı cihazlara, farklı cihaz ekranlarında düzgün görünen kodlar yazmaya çalışıyor. Her ekranın genişliği boyutları farklı olduğu için tek bir ekran türüne göre tasarım ve kodlama yapmak da bu sorunu çözmüyor. Bu yüzden farklı cihazlarda da iyi görünen siteler yapmak için temel görünen alanı, bu alanın genişliğini vs tanımlamamız gerekiyor. İşte viewport burada yardımımıza koşuyor.
    
    ```
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    ```
    
    Burada genişliğin cihaz genişliğinde olduğunu ve zoom oranının 1.0 olacağını tarayıcıya belirmiş oluyoruz. Böylece mobilde masaüstü görünümü gibi bir görünüm değil olması gerektiği gibi düzgün bir görüntü elde ediyoruz. Detaylı bilgi için şurayı inceleyebilirsiniz : https://fatihhayrioglu.com/meta-viewport-etiketi/
    
    Şimdiye kadar başlık etiketlerini, başlık etiketlerinin özelliklerini ve genel kullanım alanlarını öğrenmiş olduk.
    
- **Şimdi sıra kısa bir alıştırma yapalım. Lütfen soruları cavaplarken kendinize biraz zaman tanıyın ve yukarıdaki bilgilere göre hareket edin.**
- **Bu bilgiler :**

→ Web sitesinde en çok kullanılan baskın renk nedir? (`dominantColor`) → Sayfanın başlığı nedir? (`title`) → Sayfanın açıklaması/konusu ne üzerinedir? (`description`)

Bu verilerin sayfadan kolayca alınabilmesi için hangi etiketler hangi özelliklerle nasıl kullanılmalı?

**Cevaplar :**

1. CDN (Content Delivery Network) yardımıyla bootstrap stil ve js dosyalarını sayfamıza eklemek istiyoruz. Bunun için google'da bootstrap cdn diye arattığımızda karşımıza yukarı öğrendiğimiz link ve script etiketleriyle bootstrapi nasıl ekleyebileceğimiz çıkıyor. link etiketimizde integrity özelliğimizle imza kontrolü yaptığımıza crossorigin özelliğimizi kullandığımıza ve ilişkilendirme(rel/relation) türünün stylesheet olduğuna dikkat edin. Script etiketimizde de aynı özellikler bulunmakta :

```
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z" crossorigin="anonymous"><script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js" integrity="sha384-B4gt1jrGC7Jh4AgTPSdUtOBvfO8shuf57BaghqFfPlYxofvL8/KUEfYiJOMMV+rV" crossorigin="anonymous"></script>

```

1. Bu tip sayfayla ilgili veriler için `<meta>`etiketini kullandığımızdan bahsetmiştik. Ayrıca başlık için de `<title>`etiketini kullandığımızı söylemiştik. Şimdi bu etiketlerin doğru kullanımlarına bakalım :

```
<title>Kodluyoruz HTML</title> <meta name="dominantColor" content="red">
<meta name="description" content="Kodluyoruz ile webe giris">

```

## 4) VS Code ile Çalışmak  ve İlk HTML Sayfasınıın Web Tarayıcıda Gösterilmesi

- [x]  Yapıldı

## 5) Açıklama Satırları Oluşturmak

- Kendimize not almak için veya koddaki kısımları açıklamak için kullanabiliriz.
- Web sayfalarımızı hazırlarken açıklama satırlarını nasıl oluştururuz, hangi durumlarda kullanırız, amacı nedir bu açıklama satırlarının gibi konuları inceliyor olacağız.
- Web sayfalarımızı hazırlarken bazı durumlarda açıklama satırlarına ihtiyaç duyarız. Eğer HTML'e başlamadan önce herhangi bir yazılım dili ile ilgilendiyseniz yorum/açıklama satırlarını kullanmışsınızdır. HTML tarafında açıklama satırlarının yazım stili diğer dillere göre daha farklı.
- **Açıklama satırı eklemeli miyim?**
    - Evet, eklemelisin. Çünkü açıklama satırlarını kodunuzu 2 ay sonra tekrar gözden geçirmek için açtığınızda neyin nerede olduğunu anlamanız açısından fayda sağlayacaktır. Sadece kendimiz ile de bitmiyor. Projeyi farklı bir kişiye devrettiğinizde veya paylaştığımızda yazdığınız yorum satırlarının başka biri tarafından okunması karşı taraf için de fayda sağlayacaktır. Hatta yazdığımız kodların reçetesi veya ilacın üzerine yazılan kullanım talimatı gibi yorumlayabiliriz. :)
- **Açıklama satırı nasıl oluşturulur?**
    - Açıklama satırını HTML kodumuzda `<!–` ile başlatıp `–>` ile bitecek şekilde yazabiliyoruz. "ile başlatıp" yazan alana yorumlarımızı ekleyebiliyoruz.
- **Açıklama satırı web sayfasında görünür mü?**
    - Hayır, kullanıcılar web sayfanızda açıklama satırlarını görmezler. Ayrıca açıklama satırları web tarayıcıları tarafından herhangi bir işleme tabi tutulmazlar. Fakat kullanıcı sayfanızda sağ tıklayıp kaynağı görüntüle dediğinde açıklama satırlarınızı görebilir.
- **Hadi örneklendirelim!**
    - Aşağıdaki örnekte birden fazla HTML elementlerini tanımlayıp aralara açıklama satırları ekliyoruz. Böylelikle HTML kodumuz daha okunabilir bir hal alabiliyor. Hangi elementin nerede kapatıldığını veya açıklama satırına yazacağımız o kodun işlevi ile daha açıklayıcı bir hale getiriyoruz. Aşağıdaki örnekte **index.html** dosyasının body elementi içerisine yazacağımız kodları paylaşıyorum.
        
        ```
        <!--nav element başlangıç--> <nav>
            <ul>
                <li>Anasayfa</li>
                <li>Kurumsal</li>
                <li>İletişim</li>
            </ul>
        </nav>
        <!--nav element bitiş-->
        
        <!--section element başlangıç-->
        <section>
            <p>Lorem Ipsum, dizgi ve baskı endüstrisinde kullanılan mıgır metinlerdir.</p>
        </section>
        <!--section element bitiş-->
        
        <!--footer element başlangıç-->
        <footer>
            Copyright © 2021
        </footer>
        <!--footer element bitiş-->
        
        ```
        

## 6) Başlıklar ve Paragraflar ile Çalışmak

## **HTML Paragrafları**

HTML'de **enter** işlevi yoktur. Bu yüzden eğer farklı farklı paragraflar oluşturmak istiyorsak `<p>` etiketini kullanırız. Bir paragraf her zaman yeni bir satırda başlar ve tarayıcılar bir paragrafın önüne ve arkasına otomatik olarak biraz beyaz boşluk (kenar boşluğu) ekler.

```
<p>This is a paragraph.</p> <p>This is another paragraph.</p>

```

## **HTML Başlıklar**

HTML’de en önemli kısım başlıklardır. `<h1>` Etiketi yazıların başlık şeklinde yazılması için kullanılır. Altı tane başlık çeşidi vardır. Bu başlık özellikleri `<h1>` den `<h6>` ya kadar kodlanmıştır. `<h1>` Etiketi en büyük fontu ve en çok önemi bildirirken `<h6>` ya doğru azalma göstermektedir.

```
<h1>H1 Başlık</h1> <h2>H2 Başlık</h2>
<h3>H3 Başlık</h3>
<h4>H4 Başlık</h4>
<h5>H5 Başlık</h5>
<h6>H6 Başlık</h6>

```

### **HTML Görünümü**

! [](https://user-images.githubusercontent.com/74019386/103456246-57e91380-4d05-11eb-8bc3-0c6566057f58.PNG)

Başlıklar HTML Dökümanlar’da büyük önem arz eder. Arama motorları, web sayfalarınızın yapısını ve içeriğini indekslemek için başlıkları kullanır. Kullanıcılar genellikle başlıkları ile bir sayfayı gözden kaçırırlar. Belge yapısını göstermek için başlıkları kullanmak önemlidir. `<h1>`Başlıklar ana başlıklar için kullanılmalı, ardından başlıklar takip edilmeli `<h3>`, biraz daha az önemli `<h4>`vb.

Kaynak:

• [w3schools.com](https://www.w3schools.com/html/html_paragraphs.asp)

• [html.com](https://html.com/paragraphs/)

## 7) ****Listeleme Etiketleri****

Listeleri iki ana başlık altında listeleyebiliriz;

1. Sıralı Listeler
2. Sırasız Listeler

## **Sıralı Listeler**

Sıralı listeler ardışık liste numaraları vermek için kullanılır. Sıralı listelerden yararlanmak için `<ol>` etiketi kullanılır.

```
<p> Gerçek <b>tereyağı</b> nasıl anlaşılır ?</p>     <ol>
        <li>Oda sıcaklığında tamamen erimez</li>
        <li>Suyun içinde tek parça halinde çözünür</li>
        <li>Tereyağı rengi sarı yada beyaz olabilir</li>
    </ol>

```

**Ekran çıktısı:**

!https://github.com/Kodluyoruz/taskforce/raw/main/html/listelerle-calismak/figures/s%C4%B1ra.PNG

şeklinde olur.

Liste başındaki sıralandırmayı rakamdan başka **roma rakamı veya alfabetik** şeklinde de yapabiliriz. Bunun için **type**özelliğini kullanmamız gerekir.

```
<ol type="I">   <li>Javascript</li>
  <li>C#</li>
  <li>Php</li>
</ol>

```

**Ekran çıktısı:**

!https://github.com/Kodluyoruz/taskforce/raw/main/html/listelerle-calismak/figures/siralama.png

```
<ol type="A">   <li>Javascript</li>
  <li>C#</li>
  <li>Php</li>
</ol>

```

**Ekran çıktısı:**

!https://github.com/Kodluyoruz/taskforce/raw/main/html/listelerle-calismak/figures/alfabetik.PNG

## **Sırasız Listeler**

**Sırasız listeler** numaralandırma olmadan oluşturduğumuz listeleredir. Her bir liste elemanı bir satırı kaplayacak şekilde yani blok etiket şeklinde oluşturulur.

```
<ul>   <li>Çay</li>
  <li>Türk Kahvesi</li>
  <li>Süt</li>
</ul>

```

**Ekran çıktısı:**

- Çay
- Türk Kahvesi
- Süt

şeklinde olur. Liste elemanlarının başındaki içi dolu daireyi değiştirebilir veya silebiliriz.

- *Silmek İçin: **

```
<ul style="list-style-type:none">   <li>Çay</li>
  <li>Türk Kahvesi</li>
  <li>Süt</li>
</ul>

```

**Ekran çıktısı**:  Çay

 Türk Kahvesi

 Süt

şeklinde olur. Liste başındaki içi dolu daireyi değiştirmek için ise **disc, square, circle** değerlerini kullanabiliriz.

```
<ul style="list-style-type:square">   <li>Telefon</li>
  <li>Bilgisayar</li>
  <li>Yazıcı</li>
</ul>

```

**Ekran çıktısı:**

!https://github.com/Kodluyoruz/taskforce/raw/main/html/listelerle-calismak/figures/kare.PNG

## 8) Emmet İle Daha Hızlı HTML Yapıları Oluşturmak

Emmet web geliştiricilerinin sıklıkla zamandan tasarruf etmek ve daha hızlı kod yazmak için kullandığı bir eklentidir. Emmet’in temel mantığı, yazılımcıya kodlama yaparken zaman kazandırmasıdır. Örneğin hepimiz bir html dosyasının iskeletini biliriz:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
</body>
</html>

```

Emmet sayesinde çok daha hızlı bir biçimde `!` + Tab kullanarak bu yapıyı oluşturabilirsiniz. Bunu tek tek yazmaktansa iki tuşa basarak yapmak çok güzel değil mi?

https://camo.githubusercontent.com/2b6b8cc6da640800e1cb752bce4fbb8ec4d96ec3988d09ac9a7c5a736f35b49e/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f3836352f302a74494c593447596a427670466f355a782e676966

Anlayacağınız üzere Emmet bazı kısa yollarla basit bir biçimde HTML ve CSS kodu yazmamıza yardımcı olur. Aynı kodu tekrar tekrar yazmanızı engellerken üretkenliğinizi de arttırmış olur. Emmet neredeyse tüm text editörlerinde mevcuttur, bu yüzden onu yüklemenize gerek yoktur. Ama herhangi bir nedenden IDE’nizde mevcut değilse [bu sayfadan](https://emmet.io/download/) yükleyebilirsiniz.

## **Emmet’deki Kısa Yollara Gelecek Olursak...**

Emmette kullandığımız bazı kısa yollar var, şimdi bunları örnekleriyle tek tek inceleyelim.

1 - `>` ifadesini kullanarak kardeş element oluşturuyoruz.

Örneğin şekildeki, gibi `ul` tagı içerisinde `li` tagı oluşturmak istiyorsunuz. Bunun için yapmanız gereken tek şey `ul>li` yazarak Tab’a basmak.

```
<ul>
  <li></li>
</ul>

```

Bu işlemi yaptıktan sonra ul tagına eklemek istediğimiz bir kardeş eleman kalmayınca ise `^` ifadesini kullanarak `ul`tagı dışına çıkıp yeni taglar oluşturabiliriz.

Örneğin `ul` tagı içinde `li` tagı oluşturduktan sonra `ul` tagı dışında bir `p` tagı eklemek istiyorum. Bunun için `ul>li^p`yazarak taba basabilirim.

```
<ul>
    <li></li>
</ul>
<p><p/>

```

2 - Peki ya bu `ul` tagı içerisine birden fazla `li` oluşturmak istiyorsam, ne yapmalıyım?

Bunun için `*` ifadesini kullanırız. `ul>li*3` yaparak `ul` tagı içerisinde üç adet `li` tagı oluşturabilirsiniz.

```
<ul>
  <li></li>
  <li></li>
  <li></li>
</ul>

```

3 - Bunu yerine benzer biçimde kardeş eleman-tag eklemek için `+` ifadesi de kullanılabilirdi: `ul>li+li+li`

4 - Tag eklerken onlara class özelliği vermek için de `.` ifadesini kullanırız.

Örneğin `ul.class1>li.class2` yazılarak tab tuşuna basıldığında:

```
<ul class="class1">
    <li class="class2"></li>
</ul>

```

Bu şekilde bir kod oluşur. Aynı şekilde `ul.class1>li.class2*3` denerek bir yerine üç adet class2 sınıfından `li`tagı oluşturulabilirdi.

5 - Bir id özelliği eklemek için ise `#` ifadesini kullanırız. Yeni bir örnekle id özelliği eklemeyi görelim. `ul#id1>li#id2`diyerek aşağıda gördüğünüz kodu oluşturabiliriz.

```
<ul id="id1">
    <li id="id2"></li>
</ul>

```

6 - Burada `+` ve `*` ifadesinin farkını da daha kolay anlayabiliriz.

Örneğin `ul` tagının içine aynı id’ye sahip 3 adet `li` eklemek istiyorsam `*` ifadesi kullanılabilir.

Fakat amacım farklı `id`’lere sahip üç adet `li` tagı oluşturmaksa `ul>li#id1+li#id2+li#id3` yapılır.

7 - Peki otomatik artış sağlayan değerleri tek tek yazmak amacımız zaman tasarrufu iken ne kadar mantıklı?

Emmet bunun için de bir kısa yola sahip :`$` ifadesi. Yani yukarda görmüş olduğunuz `ul>li#id1+li#id2+li#id3`şeklinde yazdığımız kod bloğunu çok daha basit bir biçimde `ul>li#idNo$*3` diyerek yazabiliriz.

Böylece otomatik olarak `idNo1`, `idNo2` ve `idNo3` idlerine sahip üç adet `li` tagımız olur.

```
<ul>
  <li id="idNo1"></li>
  <li id="idNo2"></li>
  <li id="idNo3"></li>
</ul>

```

8 - Sırada oluşturulan tagların içine text yazılması var:

Textlerimizi `{}` ifadesinin içine yazmamız yeterli: `p{Emmet ile tag içine text yazma}`

```
<p>Emmet ile tag içine text yazma</p>

```

9 - Bir diğer emmet kısa yolunu ise kodumuzda içerik olmadığı zamanlarda kullandığımız anlamsız yazıları yani **“lorem ipsum”ları** oluşturmak için kullanıyoruz.

Örneğin bir paragraf oluşturacaksınız ve bu paragrafın henüz bi içeriği yok fakat boş durmasındansa oraya metin geleceğini belirtmek istiyorsunuz veya metin geldiğinde nasıl görüneceğini görmek istiyorsunuz. Anlamsız harfler veya zaman gerektiren rastgele cümleler oluşturmak yerine bu kısayolu kullanabilirsiniz : `p>lorem` Taba bastığınızda aşağıdaki gibi bir çıktı alacaksınız.

```
<p>Lorem ipsum dolor sit, amet consectetur adipisicing elit.Facere dolore sint ea? Molestiae ratione ullam, illo commodi ipsum soluta mollitia itaque,maiores maxime natus reiciendis architecto. Quaerat culpa beatae dicta.</p>

```

10 - Bu kadar uzun bir lorem yazısı istemiyorsanız yapmanız gereken tek şey `lorem` yazdıktan sonra yanına kaç kelimeli bir lorem oluşturmak istediğinizi eklemek.

**Örneğin 5 kelimeli bir lorem yazısı istiyorsunuz.** Bunun için `p>lorem5` yazmanız yeterli.

```
<p>Lorem ipsum dolor sit amet.</p>

```

11 - Son olarak Emmet’in bir özelliğinden bahsedeceğim. `li.className` yazıp Tab’a bastığımızda ne oluşmasını bekleriz?  **Evet** `className` class’ına ait bir `li` tagı oluşmasını. peki herhangi bir tag koymaksızın sadece `.className` yazdıktan sonra Tab’a basarsak ne olur?

Cevap:

```
<div class="className"></div>

```

Gördüğünüz gibi bir `div` oluşturdu. Emmet’e bir tag vermeksizin `.` veya `#` ifadelerini kullandığımızda bunun `div` tagı olduğunu biliyor.

Ama biz bunu ul tagı içinde denersek tepkisi ne olur? **Hadi deneyelim!:**

```
<ul>
  <li class="className"></li>
</ul>

```

Gördüğünüz gibi `ul>.className` yazıp Tab’a bastığımızda ise bunun `li` elementi olduğunu algılıyor.

Emmet’in kendi sitesindeki cheat sheete  [buradan](https://docs.emmet.io/cheat-sheet/) ulaşabilirsiniz. Bu konuda bol bol egzersiz yapmayı unutmayın lütfen, emin olun başta eliniz alışana kadar çok zorlansanız da emmet kullanımı çalışma hızınızı arttıracak ve sizi gereksiz çabadan kurtaracaktır.

## **Kaynaklar**

- [Why I love pressing tab, featuring Emmet](https://medium.com/doctolib/why-i-love-pressing-tab-featuring-emmet-578aa4e77858)

## 9) Görsellerle Çalışmak

Merhaba arkadaşlar bu yazıda HTML belgesine resim ekleme , bu resimlerle çalışma konusunu inceleyeceğiz. Öncelikle HTML sayfasına resim eklemek için `<img>` tagi kullanılır.

## **`src=""` Kullanımı**

Kod bloğundaki `src=""` özelliğine görselin URL ya da dosya adresi belirtilerek resim HTML sayfasına çağırılır. (Resmi webden çağırmak için resmin URL'ini src=”…” parametesine eklemek yeterlidir.)

```
<img src="ornek.jpg"/>

```

Yukarıdaki örnekte resim HTML dosyasıyla aynı dizinde(klasörde) olduğu için direkt adını ve uzantısını yazmak yeterlidir. Burada img uzantısına dikkat etmek önemli, HTML dosyaları nasıl **.html** ile bitiyorsa tüm resim dosyalarının sonu da **.xbm, .gif, .png veya .jpg** ile veya başka bir resim formatıyla bitmelidir.

### **Yaygın Image Formatları**

Diyelim ki projenin içerisinde bir dizin oluşturdunuz (images) ve resminizi bu dizine eklediniz. Bu defa çağırmak için öncelikle images dizinine gitmek gerekiyor.

```
<img src="images/ornek.jpg"/>

```

Ya da resim bir üst dizinde kalıyor olabilir. Bu durumda bir üst dizine çıkıp images dizinini bulup resmi çağırmak gerekiyor. **(Üst dizine çıkmak için ../ kullanırız.)**

```
<img src="../images/ornek.jpg"/>

```

Bu şekilde istediğiniz kadar üst dizine çıkabilirsiniz.

```
<img src="../../images/ornek.jpg"/>

```

## **`alt=""` Kullanımı**

Alt textlerin temel amacı, görüntüleri göremeyen kullanıcılar için metinler sunmaktır. Kullanıcı görseli görüntüleyemez ise (Yavaş bağlantı, src özelliğinde hata vb.) alt özelliği görüntü için alternatif bilgilendirici bir metin içerir.

```
<img src="../images/kedi.jpg" alt="Yavru Kedi"/>

```

## **`title=""` Kullanımı**

Title özelliği kullanıcıyı bilgilendirme amacı taşır. `Cursor`(mouse imleci) ile görselin üzerine gelince bu özelliğe verilen text mesajı görünür. Ek açıklama gerektirecek resimlerde kullanabiliriz. Bilgilendirme amacı taşır.

```
<img src="../images/kedi.jpg" title="image"/>

```

**NOT**: *Title ve Alt parametreleri SEO açısından önem taşımaktadır.*

## **`width` ve `height` Kullanımı**

Görsele istenen ölçüleri vermek için `width` ve `height` özellikleri kullanılır.

**Width yatay genişlik, Height ise dikey uzunluk** için kullanılır.

Width ve Height özellikleri tanımlanmadığı zaman görsel sayfada gerçek ölçüleri ile görünür. Bu ölçülerden yalnızca birine değer verildiğinde görsel oranları korunarak belirlenen ölçüde görünür. Her iki özelliğe de değer verildiğinde resim oranları yeni verilen ölçülerde olduğu gibi görünür. Bu kullanım resim ölçüleri ile uyumlu olmadığı zaman resimde oransal bozukluklar oluşur.

```
<img src="resim.jpg" width="300" />
<img src="resim.jpg" height="400" />
<img src="resim.jpg" width="300" height="600" />
<img src="resim.jpg" height="100%" />

```

[Buradan](https://jsfiddle.net/detfj6w9/4/) örneği inceleyebilirsiniz.

## **`border` Kullanımı**

Görseli belirtilen kalınlıkta çerçeve içine alır. Daha gelişmiş **CSS Border** özelliği bunun yerine kullanılabilir.

Aşağıda `border` örneği: Görsele **3 pixel** kalınlıkta border verir.

```
<img src="resim.jpg" border="3" />

```

## **`align` Kullanımı**

Web sayfasında resmin gözükeceği pozisyonu belirlemede align özelliği kullanılır. Bu özelliğe verilebilecek değerler şunlardır: `left`, `right`. Görselin sağa veya sola yaslı çıkmasını sağlar.

```
<img src="resim.jpg" align="right" />

```

## **Görsele Link Vermek**

Görsele link vermek için `img`tag'i `a` taginin içerisinde kullanılır. Yönlendirilmek istenen yerin URL'i `a` taginin `href` özelliğine yazılır. Görsel ise `a` taginin açıklama kısmına eklenir.

```
<a href="default.asp">
  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a>

```

[Buradan](https://jsfiddle.net/qcpfsev7/2/) örneği inceleyebilirsiniz.

## **`map` ve `area`**

Görselleriniz *hyperlink* atamanız durumunda görselin tüm alanı link alanı haline dönüşecektir. Görselin herhangi bir yerine tıklanılması durumunda görsel sizi tanımlanan bağlantıya gönderecektir. `<img>` etiketleri için kullanılan `<map>` ve `<area>` etiketleri ile resmin içindeki koordinatlarla belirlediğimiz bir alanı sadece link haline getirebiliriz. Eklediğimiz `<area>` etiketi kadar belirlenen alanı bir resim üzerinden birçok bağlantıya link verebiliriz.

**Örneğin** Instagram'da bazı satıcılarda gördüğünüz bir insan fotoğraf üzerinde pantolon ve ayakkabının ürün linklerini ayrı ayrı vermek isterseniz kullanabilirsiniz.

```
<html>
<body>
<img src="workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">

<map name="workmap">
 <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm">
 <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm">
 <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="coffee.htm">
</map>
</body>
</html>

```

[Buradan](https://www.w3schools.com/html/tryit.asp?filename=tryhtml_images_map2) inceleyebilirsiniz.

## **`onload` Event'i Kullanımı**

Bu olay görsel yüklenmesi tamamlandığında çalışacak fonksiyonu belirler. *Herhangi bir nedenle görsel yüklenemezse ya da belirtilen adreste resim yoksa fonksiyon çalışmaz.*

Aşağıdaki örnekte görsel yüklenmesi tamamlandığında `resimYuklendi()` fonksiyonu çalışacak ve ekrana **Resim Yüklendi.** uyarısı JavaScript tarafından bastırılacak. Bu konuyu ileride çok daha detaylı göreceğiz.

```
<html>
    <body>
        <img src="resim.jpg" onload="resimYuklendi()" />
    </body>

    <script>
        function resimYuklendi(){
            alert("Resim yüklendi.");
        }
    </script>
</html>

```

## **`picture` Elementi ile Kullanım**

HTML5 ile gelen `picture` elementi web sayfamızda responsive image'ler kullanmamız konusunda büyük kolaylıklar sağlıyor. Bir tane `img` ve birden fazla source içerebilir. `picture` tagi ekran boyutlarına göre birden çok source kulllanmamızı sağlar bu sayede ekran boyutu değiştikçe farklı image'leri kullanabilirsiniz.

**Örnek:** Burada ekran genişliğinin 800 pikselden küçük olduğu durumlarda başka diğer koşullarda ise başka bir görsel kullanılacak.

```
<picture>
    <source srcset="https://cdn.sanity.io/images/9kdepi1d/production/65c832d202a503b15d99e628f4313782f3ef50db-300x62.png" media="(min-width: 800px)">

    <img src="/media/cc0-images/painted-hand-298-332.jpg" alt="" />
</picture>

```

Tarayıcı, her bir source öğesini inceleyip eşleşme sağlar. Eşleşme bulunamazsa veya tarayıcı `<picture>` öğesini desteklemiyorsa, `<img>` öğesinin `src` URL'si seçilir. Seçilen görüntü daha sonra `<img>` öğesinin kapladığı alanda sunulur.

[Buradan](https://jsfiddle.net/a2dvm503/4/) ekran boyutunuzu değiştirerek inceleyebilirsiniz.

## 10) Linklerle Çalışmak

Bir HTML dosyası içerisinde herhangi bir sayfaya, sayfa içine, bir websitesine, e-mail, telefon adreslerine ya da dosya yolu belirtilen herhangi bir dosyaya (resim, video, zip vb.) erişmek için kullanılan HTML etiketidir. Genel yapısı `<a></a>` şeklindedir.

```
<a href="gitmek istenilen yer">Gidilecek yer için isim tanımlaması</a>

```

!https://raw.githubusercontent.com/Kodluyoruz/taskforce/main/html/linklerle-calismak/figures/a-tagi.png

## **HTML sayfaları içinde kullanımı:**

### **Sayfalar arası kullanımı:**

HTML sayfalar arası geçiş yapmak için linklerden şu şekilde faydalanırız. Şu an üzerinde çalıştığımız klasörün içerisinde bir **linksayfasi.html** adında dosya oluşturduk ve içerisine bir şeyler yazdık. Şimdi HTML'de sayfalar arası linkleme ile yeni oluşturduğumuz sayfaya gitmek için link oluşturacağız:

```
<a href="linksayfasi.html">İkinci sayfaya git</a>

```

Bunu oluşturduğumuzda tarayıcı ekranımızda **Diğer sayfaya geç** diye bir link oluşacak (üzerine gelindiğinde mouse'un el işaretine dönmesinden anlaşılabilir)

**Örneği görelim:**

!https://raw.githubusercontent.com/Kodluyoruz/taskforce/main/html/linklerle-calismak/figures/sayfalar-arasi-link.gif

### **Sayfa içerisinde kullanımı:**

Sayfa içerisinde herhangi bir başlığa ya da bölüme gitmek için linkler kullanılabilir. Aynı sayfada işlem yapacağımız için birden fazla satır ekleyeceğim ve en aşağıya scroll ile kaydırmak yerine link yardımı ile gideceğim. Bunun için de gidilecek bölüm için `a` tagine `name` özelliği verilmelidir:

```
<a href="#sonbolum">Aşağı Git</a>
<a name="sonbolum"></a>

```

!https://raw.githubusercontent.com/Kodluyoruz/taskforce/main/html/linklerle-calismak/figures/sayfaici-link.gif

### **Website yönlendirmesinde kullanımı:**

`a` etiketinde `href` özelliğine verilen herhangi bir websitesi adresine kolayca gidilebilir. Burada `target` özelliğini göreceğiz. Bu özellik, gitmek istediğimiz bağlantının geçerli pencerede mi yoksa yeni bir pencerede mi açılması için kullanılır. `_self` özelliği geçerli pencerede açılması içindir. Varsayılan olarak böyledir. `_blank` özelliği ise yeni bir pencerede açılması içindir. **Kodluyoruz**'un internet sitesine gidelim:

!https://raw.githubusercontent.com/Kodluyoruz/taskforce/main/html/linklerle-calismak/figures/website-link.gif

### **Mail ve telefon yönlendirmesinde kullanımı:**

`a` etiketinin `href` özelliğine verilen `mailto:` ve `tel:` özellikleri sayesinde direkt olarak herhangi bir e-mail adresine posta gönderilebilir ya da geçerli bir telefon numarası aranabilir. **Kodluyoruz**'un e-mailine gidelim ve rastgele bir numaraya gidelim.

```
<a href="mailto:info@kodluyoruz.org">Kodluyoruz'a mail atınız.</a>
```

## 11) Blok Elementlerle ve Inline Elementlerle Çalışmak

- Inline elementler bulunduğu yer kadar alan kaplarlar.
- Blok elementler ise bulundukları alanın tamamını kaplayabilirler.
- [htmlreference.io](http://htmlreference.io) sitesinde hangi elementlerin block hangi elementlerin inline hangi elemenlerin meta ve hangi elementlerin self-closing olduğunu görebiliriz.
- https://www.codebrainer.com/blog/top-10-html-tags İhtiyacımız olabilecek 10 HTML tagi.
- div, genelde bir blok oluşturmak için kullandığımız yapıdırı.
    - Bir özelliği yoktur genelde blok açar ve sınırları belirler.
    - Bazen bir şeyleri div içerisine aldığımızda tepkisel olarak bir dönüt alabiliriz.
    - İlerleyen bölümlerde detaylı göreceğiz.
    - div’i daha iyi görebilmek için içindeki elementleri tab ile ileri alırız.
- span (`span:`)elementi hiç bir işe yaranmamış görünen sanal bir inline  kutudur.
- div blok halinde bir kutu oluştururken, span ise hayali bir kutu oluşturur belirli alanı  sadece kullanmayı sağlar.
- span ve divleri genelde css elementleri kullanırken kullanacağız.
- 

**Blok Elementler**

Blok elementler, bulundukları alanın tamamını kaplayabilen HTML elementleridir. İşte bazı örnekler:

```html
<div>
  Bu blok element bir div örneğidir.
</div>

<p>
  Bu blok element bir paragraf örneğidir.
</p>

<h1>
  Bu blok element bir başlık örneğidir.
</h1>

```

**Inline Elementler**

Inline elementler, bulundukları yer kadar alan kaplayan HTML elementleridir. İşte bazı örnekler:

```html
<span>
  Bu inline element bir span örneğidir.
</span>

<a href="<https://www.example.com>">
  Bu inline element bir link örneğidir.
</a>

<strong>
  Bu inline element bir kalın metin örneğidir.
</strong>

```

-