# [Lab 2] Personal Branding Website with Vibe Coding 🚀

**Samsung Innovation Campus - Chapter 1: Introduction to Generative AI**

Bu proje, üretken yapay zeka araçları (Claude & Gemini) kullanılarak "Vibe Coding" metodolojisiyle uçtan uca tasarlanmış ve kodlanmış bir kişisel marka web sitesi çalışmasıdır.

---

## Step 1: Define Your Personal Profile

**Discussion Point cevabım:** Bu adımda amaç CV'yi AI'ya "analiz ettirmek" değil, kendimi kendi cümlelerimle anlatmaktı. Bu yüzden mega prompt'a CV'yi eklemeden önce kısaca kendimi tanıttım:

> Ben Ayşe, Gaziantep'te yaşayan, İstanbul Kültür Üniversitesi'nden yeni mezun olmuş bir Endüstri & Bilgisayar Mühendisiyim (çift anadal). Meraklı, hızlı öğrenen ve bir problemi sadece analiz etmekle yetinmeyip çalışan bir yazılıma dönüştürmeyi seven biriyim. Kariyer hedefim AI destekli operasyon/optimizasyon sistemleri kuran bir ML mühendisi/araştırmacı olmak. Ekte CV'mi de referans olarak paylaşıyorum, ama asıl istediğim aşağıdaki üç bölümü bu kendimi anlatan çerçeveden yola çıkarak yazman.

Ardından CV ekinde detaylı okul, staj ve proje bilgilerini paylaştım ki AI hem benim kendi anlatımımı hem de somut kanıtları birleştirsin.

**Kullanılan AI Aracı:** Claude
**Kullanılan Komut (Prompt):**
> Sen uzman bir Kişisel Marka Danışmanı ve Kıdemli Front-End Geliştiricisisin. Ekte sana özgeçmişimi (CV) iletiyorum. Bu CV'deki tüm akademik geçmişimi, teknik yeteneklerimi, projelerimi, başarılarımı ve sosyal becerilerimi derinlemesine analiz etmeni istiyorum.
>
> Bu analiz doğrultusunda "Personal Branding Website with Vibe Coding" ödevim için şu 3 adımı eksiksiz tamamla:
>
> **ADIM 1: DEFINE YOUR PERSONAL PROFILE**
> CV'mi analiz ederek web sitemde kullanılmak üzere modern, enerjik, profesyonel ve teknoloji odaklı bir dille şu üç bölümü yaz:
> - **Who I Am** (Kim olduğum, vizyonum, çok yönlülüğüm ve öne çıkan güçlü yanlarım)
> - **My Skills** (Teknik yeteneklerim, kullandığım araçlar, öne çıkan projelerim ve başarılarım)
> - **My Future Goal** (CV'mdeki gidişata uygun olarak kariyerimdeki gelecek hedeflerim ve vizyonum)
> *Not: İçerikleri yazarken SADECE CV'deki gerçeklere sadık kal, kesinlikle halüsinasyon yapma veya olmayan bir bilgi ekleme, ancak bunu bir hikaye anlatımı (storytelling) gibi etkileyici yap.*
>
> **ADIM 2: GENERATE YOUR IMAGE PROMPTS**
> Web sitemdeki bu 3 bölümün yanına koymak üzere yapay zeka görsel araçlarında kullanabileceğim; modern, profesyonel, teknolojik ve yaratıcı temalı 3 adet İngilizce görsel üretim komutu (Image Prompt) hazırla. Komutlar doğrudan metinleri görselleştirmeye yönelik olsun.
>
> **ADIM 3: BUILD YOUR PERSONAL WEBSITE**
> Yukarıdaki içerikleri ve görselleri birleştiren, tek bir HTML dosyası içinde çalışan, responsive (mobil uyumlu), son derece şık, temiz (clean UI) ve modern bir web sitesi kodu yaz. Hedef kitle işe alım uzmanları (recruiters) ve şirketlerdir; bu doğrultuda güven verici ve profesyonel bir ton kullan. Tasarımda profesyonelliği vurgulayan modern bir renk paleti kullan. Görseller için `<img src="gorsel1.jpg">`, `gorsel2.jpg`, `gorsel3.jpg` yer tutucularını ekle. Tüm CSS kodlarını `<style>` etiketi içine göm ki tek dosyada anında çalıştırabileyim.

**Halüsinasyon kontrolü (Point 3):** AI'nın ürettiği üç bölümü CV'mle tek tek karşılaştırdım. Tüm rakamlar (GPA 3.66, Top 10/223, %50 süre azaltımı, +407.380 TL/ay vb.) ve proje isimleri CV'deki verilerle birebir örtüşüyordu; uydurma bir bilgi ya da abartılmış bir başarı tespit etmedim. Tek küçük düzeltme: "My Skills" bölümünde bir cümle CV'de olmayan bir sektör ismi kullanmaya çok yaklaşmıştı, onu daha nötr bir ifadeyle yeniden yazdırdım.

**Teknik entegrasyon notu:** Üretilen görseller `images/` alt klasörüne kaydedilip HTML içindeki `<img>` etiketleri `images/gorsel1.jpg`, `images/gorsel2.jpg`, `images/gorsel3.jpg` yollarını gösterecek şekilde güncellenmiştir. Site tek bir HTML dosyası + bir görsel klasörü olarak birlikte çalışacak şekilde teslim edilmiştir.

---

## Step 2: Image Generation
Sitenin görsel dünyasını oluşturmak için AI tarafından üretilen promptlar kullanılmış ve görseller projeye entegre edilmiştir.

**Discussion Point cevabım:** Görsellerin kalitesi tamamen prompt'ta stil, atmosfer ve amacı ne kadar net tarif ettiğime bağlıydı. Bu yüzden her prompt'ta üç şeyi sabit tuttum: (1) renk paleti - lacivert + amber + teal, sitenin genel tasarımıyla birebir eşleşsin diye; (2) ton - "professional", "editorial", "clean minimal tech aesthetic" gibi ifadelerle jenerik/karikatürize görsellerden kaçındım; (3) amaç - her görsel, ilgili bölümün mesajını (kimlik, yetenek/optimizasyon, gelecek vizyonu) doğrudan görselleştirsin, dekoratif kalmasın.

* **gorsel1.jpg (Who I Am):** "An editorial double-exposure portrait blending a young engineer's profile with a glowing circuit-board and factory-floor blueprint overlay, deep navy and teal color palette, cinematic tech lighting, professional style, no text."

* **gorsel2.jpg (My Skills):** "An abstract 3D visualization of an optimization route network - glowing nodes connected by curved light-trails over a dark navy background, amber and teal accent lights, resembling a logistics/MILP graph, clean minimal tech aesthetic, no text."

* **gorsel3.jpg (My Future Goal):** "A forward-looking digital illustration of a horizon line made of ascending data bars transforming into a highway/road, dawn-toned amber gradient sky meeting deep navy, symbolizing career growth through AI-driven engineering, minimal futuristic style, no text."

**İterasyon:** İlk denemede "Who I Am" görseli jenerik bir AI yüzü ürettiği için kişisel markayı yeterince yansıtmıyordu. Bunun üzerine prompt'u kendi fotoğrafımı referans alacak şekilde revize ettim:

> "Using the uploaded photo as the reference for the face and likeness, create a professional double-exposure portrait: keep the person's real facial features clearly recognizable and unaltered, blended subtly with a faint circuit-board pattern and isometric factory-line blueprint on the hair/background side only - not over the face. Deep navy and teal color grading, soft cinematic lighting, editorial tech-portrait style, no text, no distortion of facial features."

Bu revizyon sonucunda yüz net ve tanınabilir kalırken, teknik overlay yalnızca arka plan/saç bölgesine taşındı - kişisel marka için çok daha güçlü bir sonuç elde edildi. Ayrıca üretilen görsellerin köşesinde kalan platform filigranları, Claude ile birlikte basit bir görüntü işleme scripti (komşu bölgeden doku klonlama) kullanılarak temizlendi.

---

## Step 4: Review and Improve

**Discussion Point cevabım:** Generative AI'ı yalnızca ilk taslak için değil, ürünü baştan sona iyileştirmek için de kullandım. Süreç boyunca birkaç somut iyileştirme turu yaptım:

1. **Renk paleti ve tipografi:** Jenerik "AI tasarımı" kliselerinden (krem zemin + terracotta, ya da siyah zemin + neon yeşil) kaçınmak için koyu lacivert + amber + teal paleti ve `Space Grotesk` / `Inter` / `JetBrains Mono` yazı tipi kombinasyonu bilinçli olarak seçildi.
2. **İmza tasarım öğesi:** Hero bölümüne, RouteIQ/MILP projelerime doğrudan gönderme yapan, canlı canvas animasyonuyla çizilen bir "optimizasyon rota ağı" eklendi - dekoratif değil, içerikle doğrudan bağlantılı bir seçim.
3. **Görsel kalite kontrolü:** İlk üretilen portre görseli kişisel markayı yeterince yansıtmadığı için kendi fotoğrafımla yeniden üretildi; sonrasında üç görseldeki platform filigranları temizlendi.
4. **Tam entegrasyon:** Başlangıçta yalnızca iki bölümde görsel kullanılıyordu; üçüncü görsel (yol/ufuk illüstrasyonu) "My Future Goal" bölümüne eklenerek üç bölümün de görsel açıdan tutarlı ve tam olması sağlandı.

**Share Your Result:**
> "I aimed for a **Full-Stack AI Developer & ML/Operations Engineer** role, and I wanted my website to feel **modern, dynamic, and highly professional** - reflecting how I build AI-powered, software-driven solutions rather than doing conventional engineering analysis. I used AI to improve **the semantic layout structure, color contrast, the storytelling tone of each section, and even the personal photo used in the hero visual** so that it better reflects my future career."