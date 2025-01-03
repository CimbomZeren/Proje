public abstract class Kart {
    
    protected String name;
    protected String [][] anlamlar;
    
    public Kart(String name, String [][] anlamlar){
        
        this.anlamlar=anlamlar;
        this.name=name;
    }
    
    public String getName(){
        
        return this.name;
    }
    
    public abstract String[][] getAnlamlar();
    

    public String toString(){
        
        return ("Kart Ismi: "+name);
    }
}


import java.util.Date;

public class MajorArcana extends Kart{
    
    protected static String[] majorKartlar={"Joker","Buyucu","Azize","Imparatorice","Imparator","Aziz","Asiklar",
        "Savas Arabasi","Guc","Ermis","Kader Carki","Adalet","Asilmis Adam","Olum","Denge","Seytan","Yikilan Kule",
        "Yildiz","Ay","Gunes","Mahkeme","Dunya"};

    public MajorArcana(String name, String[][] anlamlar) {
        super(name, anlamlar);
    }
    
    
    
    @Override
    public String[][] getAnlamlar(){
        
        return anlamlar;
    }
    
    
    
    public String[] getKart(){
        
        return majorKartlar;
    }
    
    protected static String[][] anlamlar={
        
        //0(Joker)
        {
        "Joker, yeni baslangiclar, macera ve cesareti temsil eder. \n" +
        "Bu kart, hayatinizda yeni bir yolculuga cikmak uzere oldugunuzu \n" +
        "gosterir. Bilinmezlige adim atmak sizi hem heyecanlandirabilir \n" +
        "hem de korkutabilir, ancak bu yolculuk, buyuk ogrenme deneyimleri \n" +
        "ve firsatlar sunabilir. Hayatinizda risk almaniz ve icgudulerinize \n" +
        "guvenmeniz gereken bir donemdesiniz.",
            
        "Ask hayatinizda spontane ve heyecan dolu bir donemdesiniz. Yeni \n" +
        "bir iliskiye adim atabilir veya mevcut iliskinizde alisilmisin disinda \n" +
        "deneyimlere acik olabilirsiniz. Bu kart, ozgurluk ve bireyselligin \n" +
        "onemini vurgular. Bekarlar icin, yeni ve heyecan verici bir kisiyle \n" +
        "tanisma olasiligi vardir. Ancak, acele kararlar almadan once ne \n" +
        "istediginizi netlestirmeniz onemlidir.",
            
        "Is hayatinizda cesur bir adim atarak yeni bir projeye veya \n" +
        "kariyer yoluna baslayabilirsiniz. Bu kart, risk almanin ve yaratici \n" +
        "dusunmenin odullendirilecegi bir donemi simgeler. Ancak, planlama \n" +
        "eksikligi sizi zor durumda birakabilir. Yeni bir girisim veya is \n" +
        "degisikligi icin dogru zaman olabilir, ancak detaylara dikkat \n" +
        "etmeyi ihmal etmeyin."
        },
        
        //1(Büyücü)
        {
        "Buyucu, potansiyel, yaraticilik ve irade gucunu simgeler. \n" +
        "Bu kart, hayatinizda tum kaynaklari dogru bir sekilde kullanarak \n" +
        "hedeflerinize ulasabileceginiz bir donemde oldugunuzu gosterir. Kendinize \n" +
        "inanarak ve yeteneklerinizi sergileyerek buyuk basarilar elde \n" +
        "edebilirsiniz. Bu, manifestasyon gucunuzun yuksek oldugu bir zaman dilimidir.",
            
        "Ask hayatinizda cekim ve iletisimim on planda oldugu bir donemdesiniz. \n" +
        "Partnerinizle duygusal ve zihinsel olarak guclu bir bag kurabilirsiniz. \n" +
        "Bekarlar icin, karizmatik ve etkileyici bir kisiyle tanisma olasiligi \n" +
        "yuksektir. Ancak, iliskide manipülasyon veya yaniltici davranislardan \n" +
        "kacinmaniz onemlidir",
            
        "Kariyerinizde yaratici fikirlerinizi hayata gecirmek ve basariya \n" +
        "ulasmak icin gereken tum yeteneklere sahipsiniz. Bu kart, dogru \n" +
        "kaynaklari ve araclari kullanarak buyuk projelere imza atabileceginizi \n" +
        "gosterir. Liderlik ve stratejik dusunme, is hayatinda sizi one \n" +
        "cikartacaktir. Ancak, enerjinizi dogru yonlendirdiginizden emin olun."
        },
        
        //2(Azize)
        {
        "Azize, icsel bilgelik, sezgi ve bilinmeyen sirlari simgeler. \n" +
        "Bu kart, kendinizi dinlemeniz ve ic sesinize guvenmeniz gereken \n" +
        "bir donemi isaret eder. Bilincaltinizdaki cevaplarsz ulasmak icin \n" +
        "daha derin bir anlayis gelistirebilirsiniz. Hayatinizda gizemli \n" +
        "olaylar ya da sirlar aciga cikabilir.",
            
        "Ask hayatinizda duygusal derinlik ve sezgiler on plandadir. \n" +
        "Partnerinizin gercek hislerini anlamak icin ic sesinize kulak vermelisiniz. \n" +
        "Bu kart, bir iliskinin gizli yonlerini veya sakli kalmis duygulari \n" +
        "ortaya cikarabilir. Bekarlar icin, bilinmeyen bir bagin veya mistik \n" +
        "bir cekimin ortaya cikabilecegi bir donemdir.",
            
        "Is hayatinizda sezgilerinizin size rehberlik edecegi bir \n" +
        "doneme giriyorsunuz. Kararlarinizi alirken mantik kadar icsel \n" +
        "hislerinizi de dinlemeniz onemli. Bu kart, sirlarin aciga cikabilecegini \n" +
        "ve daha fazla bilgiye ihtiyaciniz olabilecegini gosterir. Onemli \n" +
        "bir karar vermeden once detaylari gozden gecirin ve acele etmeyin."
        },
        
        //3(İmparatoriçe)
        {
        "Imparatorice, bolluk, dogurganlik ve yaratici enerjiyi temsil eder. \n" +
        "Hayatinizda uretkenligin ve buyumenin on planda oldugu bir doneme \n" +
        "isaret eder. Yeni projeler baslatmak, aile kurmak veya yaratici \n" +
        "fikirlerinizi hayata geçirmek icin mukemmel bir zamandir. Aynı zamanda, \n" +
        "doga ve cevreyle baglarinizi guclendirme arzusu hissedebilirsiniz.",
            
        "Ask hayatinizda duygusal guven ve baglilik on planda. Partnerinizle \n" +
        "iliskinizde sevgi dolu bir donem yasayabilir, birlikte guclu bir bag \n" +
        "kurabilirsiniz. Bu kart, ayni zamanda bir iliskinin buyume ve olgunlasma \n" +
        "evresine girdigini gosterebilir. Bekarlar icin, derin bir duygusal \n" +
        "bag kurabileceginiz bir kisiyle tanisma olasiligi vardir.",
            
        "Kariyerinizde uretkenlik ve basari donemi. Yaratici projelerde \n" +
        "buyuk ilerlemeler kaydedebilir ve emeklerinizin karsiligini \n" +
        "alabilirsiniz. Bu kart, ayni zamanda finansal kazanc ve \n" +
        "yatirimlarin meyve verdigi bir donemi temsil eder. Is yerinde \n" +
        "huzur ve is birligi on planda olacaktir."
        },
        
        //4(İmparator)
        {
        "Imparator, otorite, duzen ve kararliligi simgeler. Hayatinizda \n" +
        "disiplinli bir tutum sergileyerek buyuk basarilar elde edebilirsiniz. \n" +
        "Bu kart, liderlik becerilerinizin on planda oldugu bir donemi isaret eder. \n" +
        "Kurallar koymak ve hedeflerinize ulasmak icin stratejik bir \n" +
        "yaklasim benimsemelisiniz.",
            
        "Ask hayatinizda guven ve istikrar on plandadir. Partnerinizle \n" +
        "iliskinizde saglam bir temel olusturabilir, birlikte gelecege dair \n" +
        "planlar yapabilirsiniz. Ancak, iliskinizde fazla kontrolcu davranmamaya \n" +
        "ozen gostermelisiniz. Bekarlar icin, guclu ve guvenilir bir \n" +
        "partnerle tanisma olasiligi vardir.",
            
        "Is hayatinizda liderlik pozisyonuna gecebilir veya onemli \n" +
        "bir sorumluluk ustlenebilirsiniz. Bu kart, disiplin ve planlama ile \n" +
        "buyuk basarilar elde edeceginizi gosterir. Is yerinde otoritenizi \n" +
        "gostermek ve saygi kazanmak icin kararli bir durus sergileyin. \n" +
        "Ancak, esnek olmayi unutmamalisiniz."
        },
        
        //5(Aziz)
        {
        "Aziz, gelenekler, maneviyat ve bilgeligi simgeler. Bu kart, \n" +
        "hayatınızda bir rehberden veya ogretiye bagli kalarak ilerlemek \n" +
        "gerektigini isaret eder. Geleneksel degerler ve toplumsal kurallara \n" +
        "uyum saglamaniz gerekebilir. Manevi bir yolculuga cikmak veya icsel \n" +
        "bilgelik arayisi icine girmek isteyebilirsiniz.",
            
        "Ask hayatinizda baglilik ve sorumluluk on plandadir. Iliskinizde \n" +
        "guclu bir temele ve ortak degerlere dayali bir bag kurabilirsiniz. \n" +
        "Bu kart, evlilik ya da uzun vadeli bir iliski icin adim atma zamani \n" +
        "oldugunu gosterebilir. Bekarlar icin, cidi ve guvenilir bir \n" +
        "iliski arayisinda olan bir kisiyle tanisma olasiligi yuksektir.",
            
        "Is hayatinizda deneyimli bir mentor ya da rehberin destegini \n" +
        "alabilirsiniz. Bu kart, geleneksel yontemleri ve kurallari takip \n" +
        "ederek basariya ulasacagınızı gosterir. Egitim veya bilgi paylasimi \n" +
        "iceren bir proje uzerinde calisabilir ve bu surecten buyuk \n" +
        "kazanc elde edebilirsiniz."
        },
        
        //6(Aşıklar)
        {
        "Asiklar, secimler, iliskiler ve uyumu temsil eder. Hayatinizda \n" +
        "onemli bir karar verme surecine girebilir ve bu surecte kalbinizi \n" +
        "dinlemeniz gerekebilir. Ikili iliskilerde denge ve uyumu saglamak icin \n" +
        "acik iletisim onemlidir. Bu kart, hem romantik hem de kisisel \n" +
        "baglarinizi guclendirme zamaninin geldigini gosterir.",
            
        "Ask hayatinizda tutkulu ve derin bir bag kurma zamani. \n" +
        "Partnerinizle iliskinizde sevgi, uyum ve anlayis on planda olacaktir. \n" +
        "Bu kart, bir iliskinin derinlesmesi ya da yeni bir aska adim atma \n" +
        "olasiligini isaret eder. Bekarlar icin, hayatlarinda onemli bir \n" +
        "yer tutacak biriyle tanisma zamani olabilir.",
            
        "Is hayatinizda onemli bir secimle karsi karsiya kalabilirsiniz. \n" +
        "Bu kart, bir is birligi ya da ortaklik kurmanin kariyerinizde \n" +
        "olumlu bir etkisi olacagini gosterir. Ayrica, ekip calismalarinda uyum \n" +
        "ve is birligi sayesinde basariya ulasabilirsiniz. Ancak, kararlarinizi \n" +
        "alirken uzun vadeli etkilerini goz onunde bulundurmaniz onemlidir."
        },
        
        //7(Savaş Arabası)
        {
        "Savas Arabasi, zafer, irade gucu ve kontrolu simgeler. Hayatinizda \n" +
        "zorluklari asmak ve hedeflerinize ulasmak icin kararlilikla ilerledigimiz \n" +
        "bir donemi isaret eder. Bu kart, cabalarinizin karsiligini alacaginizi \n" +
        "ve disiplinli bir sekilde hareket ederek basariya ulasacaginizi gosterir. \n" +
        "Ayrica, icsel catismalarinizda dengeyi saglamaniz gerekebilir.",
            
        "Ask hayatinizda guclu bir bag ve ilerleme soz konusu. Partnerinizle \n" +
        "birlikte zorluklarin ustesinden gelebilir ve iliskinizi daha guclu bir \n" +
        "hale getirebilirsiniz. Bu kart, iliskinizde kontrol ve uyumu dengelemenin \n" +
        "onemli oldugunu hatirlatir. Bekarlar icin, guclu ve kararli bir kisiyle \n" +
        "tanisma olasiligi vardir. Ancak, duygusal derinligi yakalamak icin \n" +
        "aceleci davranmamak onemlidir.",
            
        "Is hayatinizda irade gucunuz ve kararliliginiz sayesinde basari \n" +
        "elde edeceginiz bir donemdesiniz. Zorluklarla karsilasasaniz bile, \n" +
        "disiplini elden birakmayarak tum engelleri asabilirsiniz. Bu kart, \n" +
        "liderlik becerilerinizi ve hedeflerinize ulasma yeteneginizi on \n" +
        "plana cikarir. Ancak, basariya giden yolda dengeli ve kontrollu \n" +
        "kalmaniz onemlidir."
        },
        
        //8(Güç)
        {
        "Guc karti, icsel dayaniklilik, cesaret ve sabri simgeler. \n" +
        "Bu kart, hayatinizdaki zorluklarla yuzlesirken icsel gucunuzu kullanmaniz \n" +
        "gerektigini isaret eder. Sakinlik ve sabirla hareket ederek, dis \n" +
        "dunyadaki problemleri cozebilir ve kendinizi daha guclu bir hale \n" +
        "getirebilirsiniz. Ayni zamanda, ofke veya korku gibi duygulari \n" +
        "kontrol etmeniz gerekebilir.",
            
        "Ask hayatinizda sabir ve anlayis on plandadir. Partnerinizle \n" +
        "iliskinizde guclu bir bag kurmak icin duygusal dayanikliliga ihtiyaciniz \n" +
        "olabilir. Bu kart, sevginizin zorluklar karsisinda dayanikliligini \n" +
        "gosterir. Bekarlar icin, karsilarina cikan bir kisiyle duygusal bir \n" +
        "bag kurmalari zaman alabilir, ancak bu iliski saglam bir temel \n" +
        "uzerinde gelisebilir.",
            
        "Is hayatinizda sabir ve kararlilikla hareket etmeniz gereken \n" +
        "bir doneme isaret eder. Gucunuzu gosterme ve zorluklarin ustesinden \n" +
        "gelme zamani. Bu kart, cesaretiniz ve kararliliginiz sayesinde basariya \n" +
        "ulasacaginizi simgeler. Ancak, sakinliginizi korumaniz ve aceleci \n" +
        "davranmaktan kacinmaniz onemlidir."
        },
        
        //9(Ermiş)
        {
        "Ermis, icsel arayis, yalnizlik ve bilgelik kartidir. Hayatinizda \n" +
        "bir duraklama ve kendinizi dinleme zamani geldigini gosterir. Bu kart, \n" +
        "dis dunyadan uzaklasip icsel bir yolculuga cikmayi, yasamin anlamini \n" +
        "sorgulamayi ve derin bir anlayis kazanmayi simgeler. Kendinize \n" +
        "donerek onemli cevaplara ulasabilirsiniz.",
            
        "Ask hayatinizda bir duraklama veya icsel bir degerlendirme \n" +
        "donemi olabilir. Partnerinizle iliskinizde derin dusunme ve anlam \n" +
        "arayisi on planda olabilir. Bu kart, iliskinizi daha iyi anlamak ve \n" +
        "guclendirmek icin zamana ihtiyaciniz oldugunu gosterebilir. Bekarlar \n" +
        "icin, kendi icsel yolculugunuzu tamamladiktan sonra bir iliskiye \n" +
        "hazir olabilirsiniz.",
            
        "Is hayatinizda kendi yolunuzu bulmaya ve icsel bir rehberlik \n" +
        "arayisina odaklanabilirsiniz. Bu kart, gecmis tecrübelerinizden \n" +
        "ders alarak gelecekteki hedeflerinizi belirlemeniz gerektigini gosterir. \n" +
        "Belki de kariyer degisikligi veya mevcut durumunuzu yeniden \n" +
        "degerlendirme zamani gelmistir. Sabirli olun ve aceleci kararlar almayin."
        },
        
        //10(Kader Çarkı)
        {
        "Kader Carki, degisim, donguler ve sans kartidir. Hayatinizda \n" +
        "buyuk bir donum noktasini yasayacaginiz ve beklenmedik olaylarin sizi \n" +
        "yeni bir yone goturebilecegini isaret eder. Bu kart, hem olumlu hem de \n" +
        "olumsuz degisimlere acik olmaniz gerektigini gosterir. Ancak, bu \n" +
        "degisimler uzun vadede sizin icin faydali olacaktir.",
            
        "Ask hayatinizda buyuk degisimler ve suprizler olabilir. \n" +
        "Partnerinizle iliiskinizde ani gelismeler veya yeni bir evreye gecis \n" +
        "soz konusu olabilir. Bekarlar icin, kaderin sizi yeni ve onemli \n" +
        "biriyle karsilastirabilecegi bir donemi isaret eder. Ancak, bu \n" +
        "degisimlere acik ve esnek olmaniz onemlidir.",
            
        "Is hayatinizda sans ve degisim donemi. Yeni firsatlar \n" +
        "karsiniza cikabilir veya beklenmedik bir gelisme kariyer yolunuzu \n" +
        "tamamen degistirebilir. Bu kart, firsatlari degerlendirme ve esneklik \n" +
        "gostermenin zamaninin geldigini gosterir. Hayatin dongulerine uyum \n" +
        "saglamak, basariya ulasmanizi kolaylastiracaktir."
        },
        
        //11(Adalet)
        {
        "Adalet karti, denge, durustluk ve sonuclari temsil eder. \n" +
        "Hayatinizda yaptiginiz secimlerin ve eylemlerin sonuclariyla yuzleseceginiz \n" +
        "bir donemi isaret eder. Bu kart, hem kisisel hem de evrensel adaletin \n" +
        "onemini vurgular. Kararlarinizi alirken mantikli ve adil bir \n" +
        "sekilde hareket etmeniz gerekebilir.",
            
        "Ask hayatinizda durustluk ve aciklik on plandadir. Partnerinizle \n" +
        "iliskinizde denge ve uyumu saglamak icin acik iletisim onemlidir. \n" +
        "Bu kart, iliskinizin gelecegiyle ilgili onemli bir karar alma \n" +
        "zamaninin oldugunu gosterebilir. Bekarlar icin, karsilasacaklari \n" +
        "kisinin durustluk ve guvenilirlik gibi degerlere sahip olmasi onemli olacaktir.",
            
        "Is hayatinizda adil ve mantikli bir yaklasim sergilemeniz gereken \n" +
        "bir doneme isaret eder. Bu kart, kariyerinizde gecmis cabalarinizin \n" +
        "karsiligini alacaginizi ve yaptiginiz secimlerin sonuclarinin \n" +
        "netlesecegini gosterir. Hukuki veya etik meselerde dikkatli olun \n" +
        "ve kararlarinizi titizlikle degerlendirin."
        },
        
        //12(Asılan Adam)
        {
        "Asilmis Adam, teslimiyet, perspektif degisimi ve sabir kartidir. \n" +
        "Hayatinizda bir tur duraklama veya geri cekilme donemine girdiginizi \n" +
        "gosterir. Bu, bir seyleri birakip yeni bir bakis acisi kazanmak icin \n" +
        "gereken zamani almaniz gereken bir zaman dilimidir. Beklediginiz \n" +
        "sonuclari elde etmek icin zamanin dogru olmasini beklemeniz gerekebilir.",
            
        "Ask hayatinizda sabir ve anlayis on planda. Mevcut iliskinizde veya \n" +
        "gecmisteki deneyimlerinizde bir tur derinlesme ya da yeniden degerlendirme \n" +
        "zamani olabilir. Bu kart, iliskinizden ne ogrendigine odaklanmanizi onerir. \n" +
        "Bekarlar icin, duygusal olarak olgunlasmak ve bir iliskiye \n" +
        "hazirlanmak icin zamaniniz olabilir.",
            
        "Is hayatinizda yeni firsatlar veya cozumler gormek icin \n" +
        "farkli bir acidan bakmaniz gerekebilir. Bu kart, kariyerinizde ilerlemek \n" +
        "icin geleneksel yollari bir kenara birakip daha esnek dusunmenizi onerir. \n" +
        "Isler yavas ilerliyor olabilir, ancak bu bekleyis, sonrasinda daha \n" +
        "saglam ve dogru bir yol bulmaniza yardimci olacaktir."
        },
        
        //13(Ölüm)
        {
        "Olum karti, donusum, yenilenme ve eskiyi geride birakmayi simgeler. \n" +
        "Hayatinizda buyuk bir degisim yasadiginiz ve eski aliskanliklari, dusunceleri \n" +
        "ya da yapilari birakmaniz gerektigini gosterir. Bu kart, bir donemin \n" +
        "sonu ve yeni bir baslangicin habercisidir. Korku ve direnc gosterilse de, \n" +
        "bu degisim sizi daha guclu ve olgun bir hale getirecektir.",
            
        "Ask hayatinizda onemli bir donusum yasabilir. Mevcut iliskinizde \n" +
        "ya da duygusal yasaminizda eski kaliplari birakma zamani gelebilir. \n" +
        "Bu kart, iliskinizin sona ermesi veya daha derin bir seviyeye tasinmasi \n" +
        "gibi buyuk degisikliklere isaret edebilir. Bekarlar icin, eski ask \n" +
        "kaliplarindan kurtulup yeni bir baslangic yapma zamani olabilir.",
            
        "Is hayatinizda eski projeleri ya da aliskanliklari geride birakmak \n" +
        "ve yeni bir doneme baslamak gerekecek. Bu kart, eski is iliskilerinden \n" +
        "ya da yontemlerden kurtulmanizi isaret eder. Yeniliklere acik olmaniz ve \n" +
        "donusum surecine uyum saglamaniz onemlidir. Degisim baslangicta zor \n" +
        "olabilir, ancak sonunda size buyuk firsatlar sunar."
        },
        
        //14(Denge)
        {
        "Denge, uyum ve sabir kartidir. Hayatinizda dengeyi saglama, \n" +
        "asiriliklardan kacinma ve orta yolu bulma zamani geldigini gosterir. \n" +
        "Icsel huzuru yakalamak icin dengeyi korumaniz gerekecek. Bu kart, duygusal, \n" +
        "zihinsel ve fiziksel dengenin onemli oldugunu vurgular. Sabirli ve \n" +
        "olculu bir yaklasim sergileyerek basarili olabilirsiniz.",
            
        "Ask hayatinizda denge ve uyumu saglamak icin sabirli olmalisiniz. \n" +
        "Iliskinizde asiriliklardan kacinarak orta yolu bulmaniz onemli olacaktir. \n" +
        "Partnerinizle uyum icinde olmak icin iletisimizi dengeleyin ve her iki \n" +
        "tarafin ihtiyaclarina dikkat edin. Bekarlar icin, bir iliskiye baslamadan \n" +
        "once kendi icsel dengenizi bulmaniz gerekecek.",
            
        "Is hayatinizda dengeyi saglamak icin zamana ihtiyaciniz olabilir. \n" +
        "Bu kart, sabirli ve olculu bir sekilde calisarak basariya ulasmanizi \n" +
        "gosterir. Islerinizi duzgun ve uyumlu bir sekilde duzenlemek, uzun vadede \n" +
        "faydali olacaktir. Ayrica, asiriliklardan kacinmak ve dogru zamanlamayi \n" +
        "beklemek is hayatinizda size buyuk fayda saglar."
        },
        
        //15(Şeytan)
        {
        "Seytan karti, bagimlilik, takintilar ve sinirlamalari simgeler. \n" +
        "Bu kart, hayatinizda sizi kisitlayan, bagimli oldugunuz veya olumsuz \n" +
        "etkileyen bir durumla yuzlesmeniz gerektigini isaret eder. Seytan, dissal \n" +
        "engellerden ziyade icsel sinirlamalara odaklanir. Kendi korkulariniz, \n" +
        "takintilariniz veya aliskanliklariniz sizi engelliyor olabilir. Bu kart, \n" +
        "ozgurlestirmek ve sinirlamalarinizdan kurtulmak icin cesaret gerektirir.",
            
        "Ask hayatinizda, takintili ve bagimli bir iliski icinde olabilirsiniz. \n" +
        "Partnerinizle iliskinizde sinirlayici ve zararli bir dinamik olabilir. Bu kart, \n" +
        "iliskiyi saglikli bir duzeye tasimak icin farkindalik yaratmaniz gerektigini \n" +
        "gosterir. Bekarlar icin, eski iliski kaliplarindan kurtulmak ve saglikli \n" +
        "bir bag kurmak icin icsel gucunuzu kullanmaniz gerekecek.",
            
        "Is hayatinizda, bagimliliklar veya kucuk aliskanliklar kariyerinizi \n" +
        "olumsuz etkileyebilir. Bu kart, sizi kisitlayan ya da sinirlayan bir durumla \n" +
        "yuzlesmeniz gerektigini isaret eder. Belki de isyerinde toksik bir ortamda \n" +
        "bulunuyor olabilirsiniz. Bu durumda, ozgurlestirmek icin adim atip ve sizi \n" +
        "engelleyen durumlari asmalisiniz."
        },
        
        //16(Kule)
        {
        "Kule karti, ani degisim, yikilma ve yeniden yapilanmayi simgeler. \n" +
        "Hayatinizda beklenmedik bir olay ya da durum, temellerinizi sarsabilir ve \n" +
        "sizi duygusal, zihinsel veya fiziksel olarak sok edebilir. Ancak, bu yikim, \n" +
        "daha saglam temellerin insa edilmesi icin bir firsat sunar. Kule, eski \n" +
        "yapilari, kaliplari ve inancilari yerle bir eder, boylece dogru olani \n" +
        "bulabilmeniz icin bir bosluk yaratir. Bu kart, zorluklari, sok edici \n" +
        "olaylari ve ani degisimleri simgeler; ancak sonunda daha saglam bir \n" +
        "temel kurmak icin bir firsat sunar.",
            
        "Ask hayatinizda buyuk bir sarsinti yasabilir. Mevcut iliskiniz \n" +
        "beklenmedik bir sekilde sona erebilir ya da buyuk bir krizle karsilasabilirsiniz. \n" +
        "Ancak bu kriz, iliskideki sagliksiz dinamiklerin ortadan kalkmasini ve \n" +
        "daha saglikli bir iliskiye olanak tanir. Eger bu donemi dogru sekilde \n" +
        "atlatabilirseniz, daha derin, daha guvenli ve gercekci bir iliskiye \n" +
        "adim atabilirsiniz. Bekarlar icin de, gecmisdeki iliskilerden veya \n" +
        "kaliplarindan kurtulmak, yeni bir baslangic yapmak anlamina gelebilir.",
            
        "Is hayatinizda ani degisimler veya beklenmedik krizler olabilir. \n" +
        "Kule karti, kariyerinizdeki saglam temellerin yerle bir olabilecegini, \n" +
        "eski projelerin ya da is iliskilerinin sona erebilecegini simgeler. Bu kart, \n" +
        "bir seylerin son bulmasiyla birlikte, yeni firsatlarin dogacagina isaret eder. \n" +
        "Is yerinizde buyuk degisiklikler olabilir, ancak bu degisimlerin sonunda daha guclu ve \n" +
        "basarili bir pozisyonda olabilirsiniz. Eski dusunce ve calisma yontemlerinden \n" +
        "kurtulup daha yenilikci ve dogru bir yol izlemeye baslayabilirsiniz."
        },
        
        //17(Yıldız)
        {
        "Yildiz karti, umut, iyilesme ve ilhami simgeler. Hayatinizda taze \n" +
        "bir baslangic yapabilir ve gelecege dair umutlarinizi yeniden canlandirabilirsiniz. \n" +
        "Bu kart, zorluklardan sonra bir iyilesme donemi oldugunu gosterir. \n" +
        "Icsel baris ve guven arayisinizda basarili olabilirsiniz. \n" +
        "Duygusal ve manevi acidan sifalanma zamanidir.",
            
        "Ask hayatinizda umut dolu bir donemdesiniz. Mevcut iliskinizde \n" +
        "duygusal iyilesme ve sifalanma olabilir. Partnerinizle daha derin \n" +
        "bir bag kurma, guveni pekistirme ve romantizmi canlandirma zamani gelmistir. \n" +
        "Bekarlar icin, hayatlarinda cok umut verici bir ask firsati dogabilir. \n" +
        "Bu kart, kalbinizi acarak yeni bir aska adim atmanizi isaret eder.",
            
        "Kariyerinizde, zorluklardan sonra taze bir baslangic yapabileceginiz \n" +
        "bir donemdesiniz. Bu kart, is hayatinizda basari ve ilham getirecek yeni \n" +
        "firsatlar sunar. Içsel huzuru bulmaniz ve yeniliklere acik olmaniz \n" +
        "gerektigini gosterir. Gecmisdeki hatalarinizdan ders alarak, simdi daha \n" +
        "saglam bir temele dayali bir kariyer insa edebilirsiniz."
        },
        
        //18(Ay)
        {
        "Ay karti, sezgi, gizem ve bilincaltini simgeler. Hayatinizda \n" +
        "her seyin gorundugu gibi olmadigini gosterir. Belirsizlik, kafa karisikligi \n" +
        "ve gizemli durumlar on plandadir. Bu kart, duygusal olarak karisik ve \n" +
        "bulanik bir donem oldugunu gosterir. Sezgilerinize guvenmek ve \n" +
        "daha dikkatli olmak gerekecek",
            
        "Ask hayatinizda belirsizlik ve kafa karisikligi olabilir. Partnerinizle \n" +
        "iliskinizde tam olarak ne oldugunu anlamayabilir ya da gizli duygularla \n" +
        "karsilasabilirsiniz. Bu kart, duygusal karisikliklar ve yaniltici \n" +
        "durumlarla basa cikmaniz gerektigini isaret eder. Bekarlar icin, bir \n" +
        "iliskeye baslamak icin daha fazla netlik elde etmeniz gerekebilir.",
            
        "Is hayatinizda belirsizlik ve gizli durumlarla karsilasabilirsiniz. \n" +
        "Bu kart, is yerindeki bazi seylerin ortbas edildigini veya karmasik bir hal \n" +
        "aldigini isaret eder. Karar alirken sezgilerinizi dinlemeniz ve dikkatli olmaniz \n" +
        "onemlidir. Gizli bilgiler veya yanlis anlamalar olabilir, \n" +
        "bu yuzden dikkatli bir sekilde ilerleyin."
        },
        
        //19(Güneş)
        {
        "Gunes karti, basari, mutluluk, guven ve aciklik kartidir. \n" +
        "Hayatinizda aydinlik bir donem basladigini ve basariya dogru ilerlediginizi \n" +
        "simgeler. Zorluklar geride kalmis ve simdi huzur, nese ve basari zamani. \n" +
        "Bu kart, tum engellerin asilidini ve sansin sizinle oldugunu gosterir.",
            
        "Ask hayatinizda buyuk bir nese ve mutluluk donemi basliyor. Mevcut iliskinizde, \n" +
        "samimi iletisim ve birbirinize duydugunuz guven artacak. Bu kart, iliskinizde \n" +
        "olumlu bir degisim, taze bir baslangic ve guclu bir bag kurmanizi isaret eder. \n" +
        "Bekarlar icin, ask hayatinizda heyecan verici bir gelisme olabilir. Yeni bir \n" +
        "ilisikinin baslangici, mutlulugunuzu pekistirebilir.",
            
        "Is hayatinizda basari ve parlak bir donemdesiniz. Calismalarinizin \n" +
        "karsiligini alacak ve emeklerinizin odullerini toplayacaksiniz. Bu kart, \n" +
        "kariyerinizde önemli bir ilerleme veya taninma anlamina gelir. Is dunyasinda \n" +
        "parlak bir basari sizi bekliyor. Ayrica, isyerindeki iliskilerinizde \n" +
        "aciklik ve guven on planda olacak"
        },
        
        //20(Mahkeme)
        {
        "Mahkeme karti, uyanis, kendini sorgulama ve yeni bir baslangic kartidir. \n" +
        "Hayatinizda onemli bir donum noktasina gelmissinizdir. Gecmisdeki eylemlerinizin \n" +
        "ve kararlarinizin sonuclariyla yuzleseceksiniz. Bu kart, icsel bir \n" +
        "uyanisa isaret eder ve sizi dogru yolda ilerlemeye tesvik eder. \n" +
        "Kendinizi yeniden kesfetme zamani gelmistir.",
            
        "Ask hayatinizda gecmisdeki iliskilerden dersler alarak gelecege \n" +
        "dogru onemli bir adim atabilirsiniz. Bu kart, eski kaliplardan \n" +
        "kurtulup daha saglikli bir iliski kurmaniza yardimci olur. Partnerinizle \n" +
        "gecmisdeki hatalari, yanlis anlamalari gozden gecirebilir ve iliskinizde \n" +
        "yeni bir baslangic yapabilirsiniz. Bekarlar icin, gecmisdeki \n" +
        "iliskilerinden ders alarak dogru bir iliski kurma zamani gelmistir.",
            
        "Is hayatinizda bir uyanis ve yenilenme donemi basliyor. \n" +
        "Gecmisdeki eylemlerinizin, kararlarinizin sonuclari simdi yuzunuze \n" +
        "cikacak ve bunlarla yüzleseceksiniz. Bu kart, is hayatinizda onemli \n" +
        "bir donum noktasini, degisim ve yeni firsatlari isaret eder. Gecmisde \n" +
        "yaptiginiz hatalardan ders alarak kariyerinize yeni bir yon verebilirsiniz."
        },
        
        //21(Dünya)
        {
        "Dunya karti, tamamlanma, butunluk ve basari kartidir. Hayatinizda  \n" +
        "bir dongu sona eriyor ve buyuk bir basari elde ediyorsunuz. Bu kart,  \n" +
        "tum cabalarinizin ve calismalarinizin sonucunun geldigini, bir yolculugun  \n" +
        "tamamlandigini ve yeni baslangiclar icin hazirliginizi gosterir.  \n" +
        "Artik yeni bir asamaya gecmeye hazirsiniz.",
            
        "Ask hayatinizda buyuk bir basari, tatmin ve mutluluk donemi.  \n" +
        "Mevcut iliskinizde olgunlasmis ve butunlesmis bir bag kurmussunuz.  \n" +
        "Birlikte buyuk bir yolculuga cikabilir ve iliskinizi yeni bir asamaya  \n" +
        "tasiyabilirsiniz. Bekarlar icin, kalbinizin ve hayatinizin tamamlanacagi bir  \n" +
        "iliskiye baslama zamanidir. Bu kart, ask hayatinizda huzur ve dengeyi simgeler.",
            
        "Is hayatinizda basari ve tatmin donemi. Tum cabalarinizin  \n" +
        "karsiligini alacak ve kariyerinizde zirveye ulasacaksiniz. Bu kart,  \n" +
        "uzun suredir pesinden gittiginiz bir hedefe ulasmanizi ve bu basariyla  \n" +
        "birlikte is hayatinizda dengeli ve tatmin edici bir durum yaratmanizi simgeler.  \n" +
        "Ayrica, yeni projeler icin firsatlar da ortaya cikabilir."
        }
    };  
}


public class MinorArcana extends Kart{
    
    protected static String[] minorKartlar={"Asa Asi","Asa Ikilisi","Asa Uclusu",
        "Asa Dortlusu","Asa Beslisi","Asa Altilisi","Asa Yedilisi",
        "Asa Sekizlisi","Asa Dokuzlusu","Asa Onlusu","Asa Prensi",
        "Asa Sovalyesi","Asa Kralicesi","Asa Krali",
        
        "Kupa Asi","Kupa Ikilisi","Kupa Uclusu","Kupa Dortlusu","Kupa Beslisi",
        "Kupa Altilisi","Kupa Yedilisi","Kupa Sekizlisi","Kupa Dokuzlusu",
        "Kupa Onlusu","Kupa Prensi","Kupa Sovalyesi","Kupa Kralicesi","Kupa Krali",
        
        "Kilic Asi","Kilic Ikilisi","Kilic Uclusu","Kilic Dortlusu","Kilic Beslisi",
        "Kilic Altilisi","Kilic Yedilisi","Kilic Sekizlisi","Kilic Dokuzlusu",
        "Kilic Onlusu","Kilic Prensi","Kilic Sovalyesi","Kilic Klarlicesi","Kilic Krali",
        
        "Degnek Asi","Degnek Ikilisi","Degnek Uclusu","Degnek Dortlusu","Degnek Beslisi",
        "Degnek Altilisi","Degnek Yedilisi","Degnek Sekizlisi","Degnek Dokuzlusu",
        "Degnek Onlusu","Degnek Prensi","Degnek Sovalyesi","Degnek Kralicesi","Degnek Krali"};
    
    
    
    public MinorArcana(String name, String[][] anlamlar) {
        super(name, anlamlar);
    }

    @Override
    public String[][] getAnlamlar() {
        return kAnlamlar;
    }
    
    
    protected static String[][] kAnlamlar={
        
        //22(Asa Ası)
        {
            "Bu kart, maddi dunyada yeni bir baslangıc ve firsatlari simgeler. \n"
            + "Maddi anlamda size sunulan yeni bir yol, kariyer ya da gelir firsatlari \n"
            + "hayatiniza girebilir. Bu, somut anlamda buyume ve gelisme surecinizin \n"
            + "basladıgını gosterir. Yeni projelere baslamak, finansal durumunuzu \n"
            + "guclendirecek saglam adimlar atmak icin uygun bir donemdesiniz.",
            
            "Ask hayatinizda yeni bir baslangic ya da saglam bir iliski kurma \n"
            + "zamanı olabilir. İliskilerde guven, sadakat ve saglam bir temele dayanma \n"
            + "arayısında olabilirsiniz. Bu kart, kalici ve guclu bir iliski kurmak için \n"
            + "dogru zamanin geldigini gosterir. Bekarlar icin, hayatınıza girecek yeni \n"
            + "bir kişiyle duygusal ve maddi açıdan güvenli bir ilişkiye adım atmanız \n"
            + "olasılıklar dahilindedir.",
            
            "Is hayatinda yeni bir is ya da projeye baslamak icin mukemmel \n"
            + "bir zamandir. Bu kart, maddi anlamda buyume ve kariyerinize yatirim \n"
            + "yapma firsati sunar. Yeni bir is firsati, buyuk bir basari ya da finansal \n"
            + "bir kazanc sizin icin ufukta olabilir."
        },
        
        //23(Asa İkilisi)
        {
            "Bu kart, hayatinizdaki dengeyi bulma ve maddi ve manevi dunyalar \n"
            + "arasinda denge kurma zamani oldugunu isaret eder. Birden fazla is veya \n"
            + "sorumluluk arasinda denge kurarak, her iki alani da basarili bir sekilde \n"
            + "yonetebilirsiniz. Kararsizlik donemi geciyor, artik sorumluluklarinizi daha \n"
            + "rahat ve dengeli bir sekilde yonetebileceksiniz.",
            
            "Iliskinizde denge kurma zamani. Hem maddi hem duygusal ihtiyaclarinizi \n"
            + "birbirine entegre ederek, saglıklı bir iliski kurabilirsiniz. Bu donemde \n"
            + "partnerinizle birlikte kaynaklarinizi paylasarak daha saglam temeller uzerinde \n"
            + "bir iliski insa edebilirsiniz. Bekarlar icin, kisisel ihtiyaclarinizi ve \n"
            + "duygusal gereksinimlerinizi dengeleyerek, uyumlu bir iliski kurma firsatiniz var.",
            
            "Is hayatinda birden fazla projeyi ya da sorumlulugu dengelemek gerekecek. \n"
            + "Bu kart, islerinizi ve gunluk sorumluluklarinizi dengeli bir sekilde yurutmeniz \n"
            + "gerektigini gosterir. Cesitli gorevleri ve firsatlari bir arada tutarak \n"
            + "basarıya ulasabilirsiniz."
        },
        
        //24(Asa Üçlüsü)
        {
            "Bu kart, takım calismasi, isbirligi ve birlikte calisma gerekliligini \n"
            + "simgeler. Basari, tek basina degil, birlikte hareket ettiginiz kisilerle \n"
            + "elde edilecektir. Bu donemde, el birligiyle yapilan calismalarin meyvelerini \n"
            + "toplayacaksiniz ve baskalarinin katkilariyla daha buyuk bir basari \n"
            + "elde edebilirsiniz.",
            
            "İliskilerde isbirligi ve birlikte hareket etme zamani. Partnerinizle \n"
            + "birlikte ortak bir hedefe ulasma arzusunda olabilirsiniz. Bu kart, \n"
            + "iliskinizde daha fazla uyum ve isbirligi kurmanizi saglayacak bir \n"
            + "donem oldugunu gosterir. Bekarlar icin, baskalarindan yardim ve destek \n"
            + "alarak yeni bir iliskiye adim atma firsati dogabilir.",
            
            "Is hayatinda basari, takim calismasina dayali olacaktir. Ortak \n"
            + "projelerde ve grup calismalarinda ustun basari elde edebilirsiniz. \n"
            + "Bu kart, is arkadaslarinizla uyum icinde calısarak, buyuk bir \n"
            + "basariya ulasmaniza isaret eder."
        },
        
        //25(Asa Dörtlüsü)
        {
            "Bu kart, maddi guven ve korunma arayisini simgeler. Hayatinizdaki \n"
            + "varliklarinizi korumaya calisirken, duygusal ya da maddi kayiplar \n"
            + "yasama korkusu da olabilir. Bu donemde, varliklariniza sahip cikarken, \n"
            + "asiriya kacmamaya ozen gostermelisiniz. Kendi guvenliginizi ve \n"
            + "istikrarinizi saglamaya odaklanabilirsiniz.",
            
            "İliskilerde guvenli ve saglam temeller arayisinda olabilirsiniz. \n"
            + "Partnerinizle birlikte ortak bir gelecege yatirim yapmak isteyebilirsiniz. \n"
            + "Iliskilerde istikrar ve guven arayisiniz on planda olacaktir. Bekarlar icin, \n"
            + "kendi guvenliginizi saglama, duygusal olarak hazir hissetme \n"
            + "sureci devam ediyor.",
            
            "Is hayatinda, guvenli bir finansal temel olusturmak isteyebilirsiniz. \n"
            + "Mevcut isinizi korumak ve kazanclarinizi artirmak icin cesitli adimlar \n"
            + "atabilirsiniz. Bu kart, gelecekteki maddi guvenliginizi saglamak \n"
            + "icin istikrarlı bir yol secmenizi onerir."
        },
        
        //26(Asa Beşlisi)
        {
            "Bu kart, maddi kayiplar, zorluklar ve sikintilarla ilgili bir \n"
            + "donemi isaret eder. Yasadiginiz finansal ya da maddi krizler, duygusal \n"
            + "olarak da zorlayici olabilir. Ancak bu durum, daha iyi bir gelecege \n"
            + "ulasmak icin size degerli dersler sunacak ve yeniden ayaga \n"
            + "kalkmanizi saglayacaktir.",
            
            "Iliskide maddi ya da duygusal zorluklarla karsilasabilirsiniz. \n"
            + "Partnerinizle birlikte bu zorluklarin ustesinden gelmeniz gerekebilir. \n"
            + "Zor donemlerin ardindan iliskinizde daha guclu bir bag kurabilirsiniz. \n"
            + "Bekarlar icin, gecmisteki maddi ya da duygusal zorluklarin etkisini \n"
            + "asmak ve yeni bir baslangic yapmak zaman alabilir.",
            
            "Is hayatinda finansal zorluklar ya da kayiplar yasanabilir. \n"
            + "Ancak bu durum, gelecekte daha saglam bir maddi temele ulasmak icin \n"
            + "gecici bir donemin parcasidir. Yatirim yaparken dikkatli olmali ve \n"
            + "uzun vadeli planlar yaparak mali guvenliginizi saglamaya calismalisiniz."
        },
        
        //27(Asa Altılısı)
        {
            "Bu kart, comertlik ve karsıiikli yardimlasma donemini isaret \n"
            + "eder. Maddi ya da duygusal olarak yardim alabilir veya başskalarina \n"
            + "yardim edebilirsiniz. Bu surec, karsilikli fayda saglayan iliskiler \n"
            + "ve yardimlasmanin on planda oldugu bir donemi simgeler.",
            
            "Iliskilerde karsilikli fayda, paylasim ve comertlik on planda \n"
            + "olacaktir. Partnerinizle birbirinize destek olabilir ve iliskinizdeki \n"
            + "dengeyi saglam tutabilirsiniz. Bekarlar icin, baskalarindan alacaginiz \n"
            + "destek ile yeni bir iliskiye adim atmaniz olasidir.",
            
            "Is hayatinda, baskalarina yardim etmek ya da yardim almak \n"
            + "basarili olmanizi saglayacaktir. Bir is arkadasinizdan ya da patronunuzdan \n"
            + "alacaginiz destek, sizi hedeflerinize daha kolay ulastirabilir. \n"
            + "Ayni zamanda comert davranarak, cevrenizdeki insanlarla guclu \n"
            + "iliskiler kurabilirsiniz."
        },
        //28(Asa Yedilisi)
        {
            "Bu kart, sabir, uzun vadeli cabalar ve emeginizin karsiligini \n"
            + "alma zamani oldugunu simgeler. Bu donemde, basladiginiz isleri bitirmeniz \n"
            + "icin sabirli olmaniz gerekebilir. Maddi kazanc ve basarilar, zaman alabilir, \n"
            + "ancak cabalarinizin karsiligini alacaginiz bir donemdesiniz.",
            
            "Iliskilerde, sabirli olmaniz ve partnerinizle birlikte uzun vadeli \n"
            + "hedeflere ulasmak icin caba gostermeniz gerekebilir. Bu kart, \n"
            + "iliskinizdeki gelisim surecinin zaman alacagini, ancak sabirli ve \n"
            + "kararli oldugunuzda kalici bir basariya ulasacağinizi isaret eder.",
            
            "Is hayatinda, uzun vadeli hedefleriniz icin sabirli ve kararli \n"
            + "bir sekilde calismalisiniz. Basari, cabalarinizin karsiligini almak \n"
            + "icin zaman alabilir, ancak dogru yonu sectiginizde maddi ve \n"
            + "kariyersel anlamda kazanc saglarsiniz."
        },
        
        //29(Asa Sekizlisi)
        {
            "Bu kart, dikkatli ve ozverili calismanin simgesidir. Bugun \n"
            + "attiginiz her adim, gelecekteki basarilarinizin temelini olusturacaktir. \n"
            + "Emek ve dikkat gerektiren islerde basarili olabilirsiniz. Bu donem, \n"
            + "bir seylere odaklanarak derinlemesine calismak ve gelisim saglamak \n"
            + "icin idealdir.",
            
            "Iliskinizde daha fazla caba ve dikkat gostermeniz gereken bir \n"
            + "donemdesiniz. Partnerinize karsi olan sorumluluklarinizi yerine \n"
            + "getirerek, iliskinizin saglam temeller uzerine insa edilmesine \n"
            + "yardimci olabilirsiniz. Bekarlar icin, aski bulmak icin caba gostermeniz \n"
            + "gerekebilir, ancak sonunda istenen sonuclari elde edebilirsiniz.",
            
            "Is hayatinda cok calismaniz ve detaylara dikkat etmeniz gereken \n"
            + "bir donemde olabilirsiniz. Yaptiginiz islerin her biri, basariya \n"
            + "ulasmak icin onemlidir. Bu kart, sabirla yapilan calismalarin sonunda \n"
            + "buyuk kazanclar ve basarilar getirecegini simgeler."
        },
        
        //30(Asa Dokuzlusu)
        {
            "Bu kart, maddi basari, guven ve mutlulugun simgesidir. Maddi \n"
            + "anlamda aradiginiz guvenligi saglamis ve emeklerinizin karsiligini \n"
            + "almaya baslamissiniz. Finansal anlamda rahatlama ve istikrar donemi \n"
            + "başsliyor. Ayni zamanda, uzun vadeli guvenliginizi saglamlastirmak \n"
            + "icin attiginiz adimlarin meyvelerini aliyorsunuz.",
            
            "Iliskilerde guven ve istikrar on planda olacaktir. Partnerinizle \n"
            + "birlikte ortak bir gelecek kurmus ve duygusal acidan rahat bir donemde \n"
            + "olacaksiniz. Bu kart, iliskinizde huzur ve tatmin bulacaginiz \n"
            + "bir zamani isaret eder.",
            
            "Is hayatinda basari, guven ve finansal rahatlama donemine \n"
            + "giriyorsunuz. Calismalarinizin karsiligini almaya baslayacak ve \n"
            + "isinizde saglam temeller kurarak gelecekteki basarilarinizi \n"
            + "garanti altina alacaksiniz."
        },
        
        //31(Asa Onlusu)
        {
            "Bu kart, ailevi mutluluk, maddi guvenlik ve kalici basariyi \n"
            + "isaret eder. Maddi acidan en yuksek seviyeye ulasmis ve guvenli \n"
            + "bir yasam suruyorsunuz. Ailevi baglar guclenmis ve tum dunyadan \n"
            + "memnun bir hayat kurmussunuz. Her seyin tamamlandigi ve huzura \n"
            + "ulastiginiz bir donemi simgeler.",
            
            "Ask hayatinizda, kalici bir guven ve mutluluk soz konusu. \n"
            + "Partnerinizle birlikte hayatinizi paylasarak, maddi ve duygusal \n"
            + "olarak tatmin edici bir gelecek insa ediyorsunuz. Bu kart, \n"
            + "iliskinizde kalici bir mutlulugun gostergesidir.",
            
            "Is hayatinda finansal guvenlik ve basariya ulasmissiniz. \n"
            + "Maddi anlamda tüm hedeflerinizi gerceklectirmic ve gelecege \n"
            + "saglam adimlarla ilerliyorsunuz. Bu kart, basariyi ve guvenligi \n"
            + "simgeler, is hayatinizda her sey yolunda."
        },
        
        //32(Asa Prensi)
        {
            "Bu kart, ögrenme, firsatlar ve yeni baslangiclari temsil eder. \n"
            + "Bu kart, hayatinizda yeni bir seyler ögrenmek, becerilerinizi \n"
            + "gelistirmek veya bir hedefe odaklanmak icin bir firsatin dogdugunu \n"
            + "gosterir. Bu donem, kucuk ama saglam adimlarla ilerleyerek uzun \n"
            + "vadeli basarilar elde etmek icin harika bir zamandir. Aynı zamanda, \n"
            + "sabirli olmaniz ve detaylara dikkat etmeniz gerektigini de hatirlatir. \n"
            + "Hedeflerinize ulasmak icin planli ve caliskan bir tutum sergilemeniz onemlidir.",
            
            "Ask hayatinizda iliskiyi daha derinlemesine anlamak veya gelecege \n"
            + "yonelik planlar yapmak icin bir firsat dogabilir. Partnerinizle \n"
            + "iliskinizde guven ve istikrar olusturmak için adimlar atabilirsiniz. \n"
            + "Bekarlar icin, size karsi ciddi ve istikrarli bir yaklasim sergileyen \n"
            + "bir kisiyle tanisma olasiligi vardir. Bu kisi, iliskinin temellerini \n"
            + "saglam kurmaya onem veren biri olabilir.",
            
            "Is hayatinda yeni bir egitim, kurs ya da kariyer firsati \n"
            + "gundemde olabilir. Bu kart, yeteneklerinizi gelistirmek ve maddi \n"
            + "kazanclarinizi artirmak icin bir baslangic yapmanizi onerir. \n"
            + "Yaratici bir projeye baslama ya da kucuk caplı bir girisim uzerinde \n"
            + "calisarak ilerleme saglayabilirsiniz. Bu surecte, uzun vadeli \n"
            + "basarilar icin saglam bir temel olusturmak onemlidir; sabir ve \n"
            + "istikrar basariya ulasmanizi kolaylastiracaktir."
        },
        
        //33(Asa Şövalyesi)
        {
            "Bu kart, azim, sabir ve kararlilikla hedefe ulasmayi simgeler. \n"
            + "Her seyin adim adim ilerledigi ve somut sonuclar elde etmek icin \n"
            + "dikkatle calismaniz gereken bir donemde oldugunuzu isaret eder. \n"
            + "Bu kart, guvenilirlik ve istikrari temsil eder. Planlarinizi dikkatle \n"
            + "takip ettiginiz surece, basari sizin icin kacinilmaz olacaktir.",
            
            "Ask hayatınızda sadakat ve uzun vadeli bir baglilik on plandadir. \n"
            + "Partnerinizle birlikte guven ve saglamlik arayisinda olabilirsiniz. \n"
            + "Bu kart, iliskinizin yavas ama kararli bir sekilde gelisecegini ve \n"
            + "her iki tarafin da sabirla birbirini destekleyecegini gosterir. \n"
            + "Bekarlar icin, güvenilir bir partnerle tanisma ve uzun sureli bir \n"
            + "iliski kurma olasiligi vardir.",
            
            "Is hayatinda azim ve calikanlikla ilerleme zamani. Yavas ama \n"
            + "istikrarli bir sekilde hedeflerinize yaklasiyorsunuz. Bu kart, sabirli \n"
            + "ve planli bir calisma duzeniyle buyuk basarilara ulasabileceginizi \n"
            + "isaret eder. Projelerinizin tamamlanmasi zaman alabilir, ancak \n"
            + "sonuclar oldukca tatmin edici olacaktir."
        },
        //34(Asa Kraliçesi)
        {
            "Bu kart, maddi refah, sicaklik ve koruma hissini simgeler. \n"
            + "Bu kart, hayatiniza denge, konfor ve guven getiren bir donemi \n"
            + "isaret eder. Maddi kaynaklarinizi ve duygusal ihtiyaclarinizi uyum \n"
            + "icinde yonettiginiz bir donemdesiniz. Bu kart ayni zamanda doga ile \n"
            + "baglantı kurma ve basit yasamın keyfini cikarma zamani \n"
            + "oldugunu da gösterebilir.",
            
            "Ask hayatinizda sefkat, sadakat ve derin bir duygusal bag on \n"
            + "plandadir. Partnerinizle birlikte saglam ve guvenilir bir iliski \n"
            + "kurmus olabilirsiniz. Bu kart, partnerinizin size karsi duydugu \n"
            + "sevgiyi pratik yollarla gösterdigini ve iliskinizde huzur ve mutluluk \n"
            + "buldugunuzu isaret eder. Bekarlar icin, anlayisli ve guvenilir bir \n"
            + "kisiyle tanisma olasiligi yuksektir.",
            
            "Is hayatinda basari ve maddi guvenligi temsil eder. Calismalarinizin \n"
            + "sonuclari artik somut bir sekilde gorulmeye baslanabilir. Bu kart, \n"
            + "finansal acidan guvende oldugunuz ve kariyerinizde istikrarli bir \n"
            + "doneme girdiginizi gösterir. Ayni zamanda liderlik becerilerinizle \n"
            + "cevrenizdekilere ilham verebilirsiniz."
        },
        
        //35(Asa Kralı)
        {
            "Bu kart, maddi basari, guc ve liderligi simgeler. Bu kart, \n"
            + "guven ve kararlilikla hedeflerinize ulastiginizi ve artik diger \n"
            + "insanlara da rehberlik edebileceginizi gosterir. Maddi dunyada \n"
            + "ustalik kazanmis, kaynaklarinizi akillica yoneten ve baskalarina \n"
            + "ilham olan bir donemdesiniz.",
            
            "İliskilerde guven ve sadakat on plandadir. Partnerinizle birlikte \n"
            + "maddi ve manevi olarak istikrarli bir iliski kurmus olabilirsiniz. \n"
            + "Bu kart, iliskinizin saglam temeller uzerine kuruldugunu ve uzun \n"
            + "vadeli bir mutluluga ulastiginizi isaret eder. Bekarlar icin, \n"
            + "hayatiniza guvenilir, basarili ve koruyucu bir partner girme \n"
            + "olasiligi vardir.",
            
            "Is hayatinda zirveye ulasmis ve basariyi saglamis durumdasiniz. \n"
            + "Maddi anlamda buyuk kazanclar elde ettiginiz bir doneme girdiniz. Bu kart, \n"
            + "liderlik rolunuzu basariyla ustlendiginizi ve cevrenizdeki insanlara \n"
            + "rehberlik ettiginizi gösterir. Ayni zamanda yatirimlarinizin buyuk \n"
            + "kazanclar getirecegini de simgeler."
        },
        
        //36(Kupa Ası)
        {
            "Bu kart, duygusal bir yenilik ve kalbinizle ilgili derin bir \n"
            + "uyanisi temsil eder. Yeni bir iliski, icsel bir huzur ya da duygusal \n"
            + "bir baslangic arayisinda olabilirsiniz. Kendi duygusal ihtiyaclarinizi \n"
            + "daha iyi anlamak ve bunları hayatiniza entegre etmek, sizi yeni bir \n"
            + "sevgi ve mutluluk seviyesine tasiyacaktir.",
            
            "Bu kart, romantik bir iliskinin baslangicini isaret eder ve \n"
            + "duygusal anlamda guclu bir bag kurma potansiyeli tasir. Kalbiniz \n"
            + "saf ve acik, bu da yeni bir aska ya da iliskinize kendinizi tamamen \n"
            + "acmaniza olanak tanir. Bekarlar icin, hayatiniza girecek birinin \n"
            + "duygusal anlamda derin bir bag kurabilecegi bir donemdesiniz.",
            
            "Is hayatinda, duygusal acidan tatmin edici bir donemde \n"
            + "olabilirsiniz. Kendinizi isinizde daha mutlu ve huzurlu hissediyorsunuz, \n"
            + "bu da daha yaratici ve verimli olmaniza yol acacaktir. Is yerindeki \n"
            + "iliskilerinizde de duygusal bir denge kurarak basarili adimlar atabilirsiniz."
        },
        
        //37(Kupa İkilisi)
        {
            "Bu kart, bir iliski veya yakin bagda dengeli ve uyumlu bir \n"
            + "iletisimi simgeler. Bir kisiyle ya da durumla ilgili duygusal baginizi \n"
            + "derinlestirmeniz ve karsilikli anlayis icinde olmaniz gereken bir \n"
            + "donemdesiniz. Iki tarafli bir paylasim ve isbirligi bu donemin anahtari olacaktir.",
            
            "İliskinizde uyum ve dengeyi buldugunuz bir donemdesiniz. \n"
            + "Partnerinizle duygusal acidan birbirinize yakin ve guven dolusunuz. \n"
            + "Birlikte buyumek, iliskinizi daha saglam temeller uzerine insa etmek \n"
            + "icin harika bir zaman. Bekarlar icin, kalbinizin derinliklerine inerek \n"
            + "anlamli bir iliski kurma potansiyeliniz var.",
            
            "Is yerinde guclu bir isbirligi ya da ortaklik donemi basliyor. \n"
            + "Duygusal anlamda rahat ve uyumlu bir calisma ortami yaratmak, verimli \n"
            + "bir donemi isaret eder. Bu kart, birbirinizi destekleyerek basariya \n"
            + "ulasmaniz icin gerekli olan uyumu ve dengeyi saglar."
        },
        
        //38(Kupa Üçlüsü)
        {
            "Bu kart, kutlama, sevinc ve duygusal tatminin simgesidir. Bu kart, \n"
            + "mutlu bir birlikteligin, arkadas cevresindeki bir etkinligin ya da \n"
            + "ozel bir anin yasanacagi bir donemi isaret eder. Kalbinizde huzur ve \n"
            + "mutluluk olacak, etrafinizdaki insanlarla bu enerjiyi paylasarak \n"
            + "kendinizi daha iyi hissedeceksiniz.",
            
            "İliskinizde sevgi, anlayis ve tatmin dolu bir döneme adim atiyorsunuz. \n"
            + "Birlikte kutlayacaginiz basarilar ve mutluluk anlari, iliskinizin \n"
            + "guclenmesine katki saglar. Bu kart, partnerinizle eglenceli ve keyifli \n"
            + "bir zaman gecireceginiz bir donemi simgeler. Bekarlar icin, sosyal \n"
            + "cevredeki etkinlikler yeni bir aska zemin hazirlayabilir.",
            
            "Is yerinde bir basariyi kutlamak ya da takim calismasinin \n"
            + "getirdigi bir zafer yasanabilir. Ortak projelerde saglanan basarilar \n"
            + "ve iyi iliskiler, sizi mutlu kilacaktir. Bu donem, is arkadaslarinizla \n"
            + "birlikte kutlama yapacaginiz bir zaman dilimi olabilir."
        },
        
        //39(Kupa Dörtlüsü)
        {
            "Bu kart, bir duygusal durgunluk ve tatminsizlik hissini isaret eder. \n"
            + "Hayatinizda ya da bir iliskinizde tatmin eksikligi ya da memnuniyetsizlik \n"
            + "soz konusu olabilir. Bu durum, kendinize ve cevrenize bakis acinizi degistirmeniz \n"
            + "gerektigini gosteriyor. Kendi duygusal ihtiyaclarinizi yeniden degerlendirmek, \n"
            + "duygusal iyilesmenize yardimci olabilir.",
            
            "İliskide duygusal olarak sikismis ve tatminsiz hissedebilirsiniz. \n"
            + "Partnerinizle olan baginizi tekrar gozden gecirebilir ve iliskinize \n"
            + "yeni bir soluk getirmek icin adimlar atabilirsiniz. Bekarlar icin, \n"
            + "gecmis iliskilerden gelen duygusal acilar ya da hayal kirikliklari, \n"
            + "yeni bir baslangicin onunde engel olabilir.",
            
            "ıs yerinde, mevcut durumunuzdan memnuniyetsizlik yasayabilirsiniz. \n"
            + "Hedeflerinize ulasmak icin daha fazla caba sarf etmeniz gerekebilir. \n"
            + "Bu durum, isinizi sevmediginiz ya da tatmin olmadiginiz bir donemi isaret \n"
            + "ediyor olabilir. Yeniden degerlendirme yapmak, daha iyi bir yol \n"
            + "haritasi cizmenize yardimci olabilir."
        },
        
        //40(Kupa Beşlisi)
        {
            "Bu kart, gecmisteki kayiplar ve duygusal acilarin izlerini tasiyan \n"
            + "bir donemi temsil eder. Ancak bu kayiplar, yeniden baslayabilmek \n"
            + "ve gelecege odaklanabilmek icin bir firsat sunar. Bunu asmak icin \n"
            + "derin bir icsel yolculuga cıkmaniz ve aciyi kabul etmeniz gerekebilir.",
            
            "İliskide hayal kirikligi ve kayiplar yasanmis olabilir. Bu durum, \n"
            + "duygusal olarak zorlayici olsa da, gecmisin acilarini geride birakmak icin \n"
            + "bir firsat sunar. Yeni bir ask ya da iyilesmis bir iliski, yakin \n"
            + "gelecekte sizi bekliyor olabilir.",
            
            "Is hayatinda bir basarisizlik ya da kayiplar soz konusu olabilir. \n"
            + "Ancak bu donemde kendinizi toparlamak ve yeni firsatlari kucaklamak \n"
            + "icin guc bulmalisiniz. Gecmisteki deneyimleriniz, sizi daha \n"
            + "saglam bir temele oturtacak."
        },
        
        //41(Kupa Altılısı)
        {
            "Gecmisteki guzel anilari hatirlama ve duygusal baglari yeniden \n"
            + "canlandirma zamani. Bu kart, eski iliskilerinizi ya da gecmisteki \n"
            + "tatli anilari dusunmenizi isaret eder. Ayrica gecmisin guzel \n"
            + "taraflarini takdir ederek, simdiki zamana daha olumlu bir sekilde \n"
            + "odaklanmaniza yardimci olabilir.",
            
            "İliskinizde nostaljik bir donem baslayabilir. Eski anilari canlandirmak \n"
            + "ve gecmisteki mutlu zamanlari tekrar yasamak, iliskinizde daha guclu bir \n"
            + "bag kurmaniza yardimci olacaktir. Bekarlar icin, eski bir ask ya da \n"
            + "gecmisteki bir iliski yeniden gundeme gelebilir.",
            
            "Is hayatinizda gecmiste basariyla yaptiginiz bir ise geri \n"
            + "donme ya da eski baglantilarla yeniden isbirligi yapma donemi olabilir. \n"
            + "Bu kart, eski projelerden ya da eski is arkadaslarinizdan fayda \n"
            + "saglayabileceginizi isaret eder."
        },
        
        //42(Kupa Yedilisi)
        {
            "Bu kart, duygusal bir secim ve dikkatli kararlar almayi simgeler. \n"
            + "Hayatinizda pek cok secenek olabilir, ancak hangi yolu sececeginize \n"
            + "karar verirken dikkatli olmalisiniz. Seceneklerinizi degerlendirirken, \n"
            + "kalbinizi ve aklinizi dengelemeniz onemli olacaktir.",
            
            "İliskide bircok duygusal secenek olabilir, ancak hangi yolu sececeginiz \n"
            + "konusunda belirsizlik yasanabilir. Kendinize durust olup, hangi \n"
            + "iliski ya da kisiyle daha saglıklı bir bag kurabileceginizi \n"
            + "belirlemek bu donemin anahtaridir.",
            
            "Is hayatinda birkac secenek ya da firsat karsisinda kalabilirsiniz. \n"
            + "Ancak bunlar arasinda dikkatli bir secim yapmalisiniz. Hangi firsatin \n"
            + "size uzun vadede fayda saglayacagini gormek icin her birini \n"
            + "dikkatle degerlendirin."
        },
        
        //43(Kupa Sekizlisi)
        {
            "Bu kart, duygusal bir hayal kirikliginin ve birakmanin simgesidir. \n"
            + "Hayatinizda onemli bir seyi ya da iliskiyi geride birakmaniz gerekebilir. \n"
            + "Bu terk etme sureci zor olsa da, ilerlemek icin gerekli bir adimdir. \n"
            + "Eski baglardan kurtulmak, size daha saglikli ve yeni bir baslangic \n"
            + "yapma firsati sunar.",
            
            "İliskide duygusal tatminsizlik ve sikilma hissi yogunlasabilir. \n"
            + "Belki de iliskide eski duygular kaybolmus ve baglar zayıflamis olabilir. \n"
            + "Bu kart, bir iliskiyi terk etmek ya da eski kaliplardan cikmak icin \n"
            + "gereken gucu bulmaniza yardimci olabilir. Bekarlar icin, gecmiste \n"
            + "yasadiginiz bir iliskiyi tamamen geride birakmak ve gelecege \n"
            + "odaklanmak gerekebilir.",
            
            "Is hayatinda, sizi tatmin etmeyen bir projeyi ya da durumu \n"
            + "terk etmek gerekebilir. Eski bir isin veya gorevdeki bosluklarin sizi \n"
            + "duygusal olarak tukettigini hissedebilirsiniz. Ancak bu terk etme \n"
            + "sureci, size daha uygun ve tatmin edici yeni firsatlar yaratacaktir."
        },
        
        //44(Kupa Dokuzlusu)
        {
            "Bu kart, duygusal tatminin zirveye ulastigi ve kalbinizin huzur \n"
            + "buldugu bir donemi isaret eder. Duygusal olarak rahatladiginiz, huzur \n"
            + "buldugunuz ve etrafinizdaki insanlarla derin baglar kurdugunuz bir zaman \n"
            + "dilimi baslıyor. Basari, mutluluk ve tatmin duygusu bu donemde sizi saracaktir.",
            
            "İliskide tam anlamiyla duygusal tatmini bulmussunuzdur. Kalbinizde huzur, \n"
            + "mutluluk ve derin bir bag vardir. Birlikte paylasilan anlar, iliskinizi \n"
            + "daha guclu ve anlamli kilmaktadir. Bekarlar icin, kalbinizi acmak ve \n"
            + "saglikli bir iliskiye adim atmak icin mukemmel bir zaman dilimidir.",
            
            "Is hayatinda buyuk bir tatmin duygusu ve basari yasanabilir. \n"
            + "Yaptiginiz isler ve elde ettiginiz basarilar, sizi tatmin edecek ve \n"
            + "huzur verecektir. Is arkadaslarinizla guclu bir bag kurarak, basarili \n"
            + "bir ekip calismasi yapmaniz olasidir."
        },
        
        //45(Kupa Onlusu)
        {
            "Bu kart, duygusal bir mutluluk ve huzurun tamamlanmasidir. Aile, \n"
            + "dostlar ve yakin cevrenizle birlikte kutlayacaginiz bir mutluluk donemi \n"
            + "basliyor. Aile baglari guclenebilir ve cevrenizdeki insanlar ile aranizda \n"
            + "sevgi ve saygi dolu bir ortam olusabilir. Bu, hayatinizin en tatmin \n"
            + "edici anlarindan biridir.",
            
            "Ask ve mutluluk konusunda zirveye ulasmis bir donemdesiniz. \n"
            + "İliskinizde tam anlamiyla mutlusunuz ve partnerinizle guclu bir bag \n"
            + "kurmussunuz. Ileriye donuk saglam bir iliski icin temeller atilabilir. \n"
            + "Bekarlar icin, yeni bir aska adim atmak ve derin bir bag kurmak \n"
            + "icin mukemmel bir donemdir.",
            
            "Is hayatinda ailevi bir basari ve mutluluk donemini isaret eder. \n"
            + "Bir takim ya da is arkadaslarinizla birlikte onemli bir basariyi \n"
            + "kutlayabilirsiniz. Hem kisisel hem de profesyonel anlamda huzur ve \n"
            + "tatmin bulacaginiz bir donemin habercisidir."
        },
        
        //46(Kupa Prensi)
        {
            "Bu kart, duygusal kesif ve yeni bir ask baslangicini simgeler. \n"
            + "Kalbiniz duygusal anlamda yeni bir yolculuga cikmaya hazirdir ve yeni \n"
            + "bir sevgiyi ya da icsel huzuru kesfetmeye aciksiniz. Bu kart ayni \n"
            + "zamanda sezgisel bir uyanisi da isaret eder; kalbiniz, size \n"
            + "dogru yolu gosterebilir.",
            
            "Ask konusunda heyecan verici ve yeni bir baslangic yapabilirsiniz. \n"
            + "Kalbiniz saf ve acik, bu da yeni bir iliskiye baslamayi ya da var olan \n"
            + "iliskideki baglari derinlestirmeyi isaret eder. Bekarlar icin, hayatiniza \n"
            + "yeni bir ask girebilir ve bu ask sizi icsel bir donusume goturebilir.",
            
            "Is hayatinda yeni bir firsat ya da gorev sizi bekliyor olabilir. \n"
            + "Duygusal olarak bu is, sizi tatmin edecek ve buyutecek bir deneyim \n"
            + "olabilir. Ileriye donuk yaratici fikirler ve projeler icin de \n"
            + "uygun bir zaman dilimindesiniz."
        },
        
        //47(Kupa Şövalyesi)
        {
            "Bu kart, duygusal bir baglilik ve sevgiyi simgeler. Romantik \n"
            + "anlamda cesur bir adim atmaya karar verdiginiz bir doneme giriyorsunuz. \n"
            + "Icsel gucunuzle ve duygusal cesaretle bir adim atarak, kalbinizdeki \n"
            + "tutkulari ve hayalleri gercege donusturebilirsiniz.",
            
            "İliskide heyecanli ve duygusal bir donusum yasanabilir. Sevgilinizle \n"
            + "daha derin bir bag kurabilir ve iliskinizdeki romantizmi yeniden \n"
            + "kesfedebilirsiniz. Bu kart, askta cesaret ve guveni simgeler. \n"
            + "Bekarlar icin, kalpten bir aska adim atmaniz ve bir iliskiye cesurca \n"
            + "ilerlemeniz olasiliklar dahilindedir.",
            
            "Is hayatinda yaratici ve cesur bir yaklasim benimseyebilirsiniz. \n"
            + "Bu donemde duygusal olarak tatmin edici isler yapma, tutkularinizi \n"
            + "kariyerinize yansitma sansiniz olabilir. Ayrıca is arkadaslarinizla \n"
            + "yaratici projelerde isbirligi yaparak daha guclu baglar kurabilirsiniz."
        },
        
        //48(Kupa Kraliçesi)
        {
            "Bu kart, duygusal denge, icsel huzur ve sezgiyi temsil eder. \n"
            + "Kendinize ve cevrenize duyarli ve nazik bir yaklasim icinde oldugunuz \n"
            + "bir donemdesiniz. Kendi duygusal ihtiyaclarinizi karsilama konusunda \n"
            + "derin bir farkindalik ve anlayis gelistiriyorsunuz.",
            
            "İliskide duygusal denge ve anlayisa sahip oldugunuz bir donemdesiniz. \n"
            + "Partnerinizle guclu bir bag kurarak, ona karsi derin bir sefkat \n"
            + "ve sevgi gosteriyorsunuz. Bekarlar icin, kalpten bir iliski kurmaya \n"
            + "ve duygusal olarak tatmin edici bir bag yaratmaya aciksiniz.",
            
            "Is hayatinda sezgilerinizi ve duygusal zekanizi kullanarak \n"
            + "basarili adimlar atabilirsiniz. Hem is yerindeki iliskilerde hem de \n"
            + "kisisel projelerde, empati ve duyarliliginiz sayesinde verimli bir \n"
            + "donem sizi bekliyor. Bu kart, duygusal zekanizla onemli kararlar \n"
            + "alabileceginizi isaret eder."
        },
        
        //49(Kupa Kralı)
        {
            "Bu kart, olgunluk, duygusal denge ve liderligi temsil eder. \n"
            + "Kendinizi duygusal olarak dengede hissettiginiz ve duygusal acidan \n"
            + "guvenli bir pozisyonda oldugunuz bir doneme giriyorsunuz. Hem kendinize \n"
            + "hem de baskalarina duyarli ve nazik bir yaklasim icinde olabilirsiniz.",
            
            "İliskide olgun, guven dolu ve anlayisli bir yaklasim sergiliyorsunuz. \n"
            + "Partnerinizle duygusal anlamda derin bir bag kurmussunuz ve iliskiniz \n"
            + "saglam temeller uzerinde duruyor. Bekarlar icin, olgun ve duygusal \n"
            + "anlamda uyumlu bir iliskiye adim atma zamani olabilir.",
            
            "Is hayatinda liderlik rolu ustlenebilirsiniz. Duygusal zekanız \n"
            + "sayesinde is yerinde huzurlu ve verimli bir ortam yaratabilir, \n"
            + "insanlarla guclu baglar kurabilirsiniz. Bu kart, yonetici ve lider \n"
            + "pozisyonlarina isaret eder ve duygusal olgunlukla kararlar almayi gösterir."
        },
        
        //50(Kılıç Ası)
        {
            "Hayatinizda yeni bir fikir ya da farkindalik isigiyla onemli \n"
            + "bir baslangic yapiyorsunuz. Zihinsel netlik ve cozum uretme yeteneginiz, \n"
            + "karsilastiginiz sorunlari hizlica cozebilmenizi saglayacak. Bu kart, \n"
            + "durustluk ve mantikla hareket ederek dogru kararlar almanizi tesvik \n"
            + "eder ve basariya ulasmanin onunu acar.",
            
            "İliskinizde netlik kazanma ve durust bir iletisim kurma zamani. \n"
            + "Partnerinizle acikca konusmak, iliskinizin saglam bir temele oturmasini \n"
            + "saglayabilir. Bekarlar icin bu kart, mantikli bir sekilde dusundugunuzde \n"
            + "duygusal hayatiniza yeni bir sayfa acabileceginizi gosterir.",
            
            "Yeni bir fikir ya da zihinsel bir atilim is hayatinizda buyuk \n"
            + "bir degisim yaratabilir. Kararlarinizi analitik bir sekilde degerlendirerek \n"
            + "ilerlerseniz, basari kacinilmaz olacaktir. Bu donemde mantiginiz \n"
            + "ve zekaniz, kariyer hedeflerinize ulasmanizda en buyuk gucunuz olacak."
        },
        
        //51(Kılıç İkilisi)
        {
            "Hayatinizdaki bir kararsizlik ya da iki secenek arasinda \n"
            + "sikismislik hissi ile mucadele ediyorsunuz. Bu durum, duygularinizla \n"
            + "mantiginiz arasinda bir denge kurmaniz gerektigini gosteriyor. \n"
            + "Karar almak zor olsa da, ilerlemek icin bu durumu cozmelisiniz. \n"
            + "Uzun sure beklemek sizi daha da zor bir noktaya goturebilir.",
            
            "İliskide cozulmesi gereken bir mesele ya da alinmasi gereken bir \n"
            + "karar olabilir. Ancak su an kararsizlik icinde olmaniz nedeniyle \n"
            + "duygusal olarak tikaniklik hissedebilirsiniz. Partnerinizle acik bir \n"
            + "sekilde konusmak, bu durumu asmaniza yardimci olabilir.",
            
            "Is hayatinizda onemli bir karar asamasindasiniz, ancak secenekler \n"
            + "arasinda net bir secim yapmakta zorlanabilirsiniz. Bu karari almak \n"
            + "icin detayli dusunmeli ve her iki secenegin de sonuclarini \n"
            + "dikkatlice degerlendirmelisiniz."
        },
        
        //52(Kılıç Üçlüsü)
        {
            "Aci, hayal kirikligi ve uzuntuyu temsil eden bu kart, \n"
            + "hayatinizdaki zor bir donemi isaret eder. Ancak bu surec, duygusal \n"
            + "olarak olgunlasmaniza ve gecmisteki yaralari sarmak icin bir \n"
            + "firsat yaratir. Yasadiginiz zorluklar, ileride daha guclu bir \n"
            + "sekilde yeniden dogmaniza yardimci olacaktir.",
            
            "İliskide bir ayrilik, hayal kirikligi ya da ihanet gibi duygusal \n"
            + "acidan zorlu bir surecle karsilasabilirsiniz. Bu durum her ne kadar \n"
            + "zor olsa da, duygularinizi iyilestirerek kendinizi daha guclu bir \n"
            + "sekilde yeniden insa etmeniz mumkun.",
            
            "Is hayatinda basarisizlik ya da hayal kirikligi yasanabilir. \n"
            + "Ancak bu surec, size onemli dersler ogreterek gelecekte daha saglam \n"
            + "adimlar atmanizi saglayacaktir. Yasadiginiz bu deneyim, ilerleyen \n"
            + "sureclerde daha buyuk basarilar elde etmenize katki saglayabilir."
        },
        
        //53(Kılıç Dörtlüsü)
        {
            "Dinlenme, ice cekilme ve yenilenme zamani. Hayatinizdaki yogunluktan \n"
            + "ya da stresli durumlardan bir adim geri cekilerek, zihinsel ve \n"
            + "fiziksel sagliginiza oncelik vermelisiniz. Bu surec, enerjinizi \n"
            + "yeniden toplamaniza ve gelecege daha saglam adimlarla \n"
            + "ilerlemenize yardimci olacaktir.",
            
            "İliskide bir ara verme ya da duygusal anlamda kendinizi \n"
            + "toparlama zamani. Partnerinizle olan baginizi yeniden guclendirmek \n"
            + "icin bir sure kendinize odaklanmaniz gerekebilir. Bu mola, iliskinizde \n"
            + "daha saglıklı bir dinamik olusturmaniza yardimci olabilir.",
            
            "Is hayatinda kendinizi asiri yormus ya da tukenmis hissedebilirsiniz. \n"
            + "Bu nedenle bir sure dinlenmek ve enerjinizi yenilemek, uzun vadede \n"
            + "basarilarinizi artiracaktir. Kendinizi daha guclu bir sekilde geri \n"
            + "donmeye hazirlamalisiniz."
        },
        
        //54(Kılıç Beşlisi)
        {
            "Catisma, kayip ya da zor bir durumla karsi karsiyasiniz. \n"
            + "Ancak bu surec, size dogruyu yanlistan ayirmayi ve hayatta ileriye \n"
            + "nasil daha saglam adimlarla devam edeceginizi ogretebilir. \n"
            + "Kazandiginiz ya da kaybettiginiz seylerden bagimsiz olarak, bu \n"
            + "durumdan ders alarak ilerlemek onemlidir.",
            
            "İliskide bir tartisma ya da yanlis anlasilma, iki tarafin da \n"
            + "yipranmasina neden olabilir. Ancak bu durum, iliskinizin daha guclu \n"
            + "bir hale gelmesi icin bir firsat yaratabilir. Partnerinizle acik ve \n"
            + "durust bir sekilde iletisim kurmaniz, bu catismayi cozmenizi saglayabilir.",
            
            "Is hayatinda rekabet ya da anlasmazliklar yasanabilir. \n"
            + "Ancak bu surecte alacaginiz dersler ve gostereceginiz kararlilik, \n"
            + "kariyerinizdeki ilerlemenizde onemli bir rol oynayacaktir. Durumu sakin \n"
            + "bir sekilde ele almak size avantaj saglayabilir."
        },
        
        //55(Kılıç Altılısı)
        {
            "Zor bir donemden uzaklasarak daha sakin ve huzurlu bir surece \n"
            + "adim atiyorsunuz. Bu kart, gecmiste yasanan sikintilardan uzaklasmayi \n"
            + "ve gelecege umutla bakmayi temsil eder. Fiziksel ya da duygusal bir \n"
            + "yolculugun baslangicinda olabilirsiniz.",
            
            "İliskide gecmiste yasanan sorunlari geride birakma ve birlikte \n"
            + "daha huzurlu bir donem baslatma zamani. Bekarlar icin bu kart, gecmisteki \n"
            + "duygusal yaralarin iyilesmesiyle yeni bir iliskiye kapi acildigini gösterebilir.",
            
            "Is hayatinda yasanan stresli bir donemi geride birakiyor ve \n"
            + "daha huzurlu bir surec baslatiyorsunuz. Bu gecis, kariyerinizde yeni ve \n"
            + "olumlu bir baslangica isaret ediyor olabilir."
        },
        
        //56(Kılıç Yedilisi)
        {
            "Gizlilik, strateji ve dikkat gerektiren bir donemdesiniz. \n"
            + "Bazi durumlarda kendinizi ya da planlarinizi korumak icin daha dikkatli \n"
            + "hareket etmeniz gerekebilir. Bu kart, zeki ve stratejik olmayi, \n"
            + "ancak durustlukten sapmamayi ugutler.",
            
            "İliskide gizli kalan bir konu ya da durustluk eksikligi gundeme \n"
            + "gelebilir. Acik bir iletisim kurarak, bu durumu cozmek iliskiniz icin \n"
            + "daha saglikli bir yol acabilir.",
            
            "Is hayatinda stratejik adimlar atmaniz gereken bir donemdesiniz. \n"
            + "Gizli bir proje ya da dikkatle korunmasi gereken bir fikir üzerinde \n"
            + "calisiyor olabilirsiniz."
        },
        
        //57(Kılıç Sekizlisi)
        {
            "Kendi korkulariniz ve zihinsel sinirlamalariniz nedeniyle \n"
            + "kendinizi sikismis hissedebilirsiniz. Ancak bu sinirlamalar gercek \n"
            + "olmaktan cok, kendi dusuncelerinizden kaynaklaniyor olabilir. \n"
            + "Cesurca hareket etmeye karar verdiginizde, bu durumdan cikis yolu \n"
            + "bulabilirsiniz. Kendinizi ozgurlestirmek icin dusunce kaliplarinizi \n"
            + "gozden gecirmeniz gerekecek.",
            
            "İliskide duygusal olarak kisitlanmis ya da bastirilmis hissedebilirsiniz. \n"
            + "Bu durum, iletisim eksikliginden ya da iliskinizde hissettiginiz \n"
            + "baskidan kaynaklaniyor olabilir. Duygularinizi acikca ifade etmek, \n"
            + "iliskinizdeki bu tikanikligi asmaniza yardimci olacaktir.",
            
            "Is hayatinda bir proje ya da durum sizi sikismis ve caresiz \n"
            + "hissettirebilir. Ancak bu sinirlamalarin bircogu kendi zihinsel \n"
            + "engellerinizden kaynaklaniyor olabilir. Farkli bir bakis acisi \n"
            + "gelistirerek bu durumu asabilirsiniz."
        },
        
        //58(Kılıç Dokuzlusu)
        {
            "Korkular, endiseler ve uykusuz gecelerle dolu bir donemi \n"
            + "temsil eder. Zihinsel stres ve karamsar dusunceler, kendinizi daha da \n"
            + "kotu hissetmenize neden olabilir. Ancak bu durumun cogunlukla zihinsel \n"
            + "abartilar oldugunu fark ettiginizde, bir cozum yolu bulabileceksiniz. \n"
            + "Duygusal destek almak, bu sureci daha kolay atlatmaniza yardimci olabilir.",
            
            "İliskide endiseleriniz ve korkulariniz nedeniyle zor bir donem yasiyor \n"
            + "olabilirsiniz. Bu durum, partnerinizle acik bir sekilde konusarak ya da \n"
            + "duygularinizi anlamaya calisarak cozulebilir. Bekarlar icin bu kart, \n"
            + "gecmisteki korkularin yeni bir iliskiye baslamayi engelledigini gosterebilir.",
            
            "Is hayatinda stresli bir donemdesiniz ve belki de basarisizlik \n"
            + "ya da yanlis kararlar verme korkusu sizi etkiliyor olabilir. Ancak \n"
            + "bu endiselerin gerceklerden cok zihinsel birer kurgudan ibaret \n"
            + "oldugunu fark etmek, cozum bulmaniza yardimci olacaktir."
        },
        
        //59(Kılıç Onlusu)
        {
            "Zor bir sonlanma ya da hayal kirikligini temsil eder. Hayatinizin \n"
            + "bir alaninda artik tamamen biten bir durumla karsilasabilirsiniz. \n"
            + "Ancak bu son, yeni bir baslangicin yolunu acacaktir. Her ne kadar \n"
            + "aci verici olsa da, bu surec size dayaniklilik kazandirarak \n"
            + "gelecekte daha guclu olmanizi saglayacaktir.",
            
            "İliskide sona erme ya da agir bir hayal kirikligi yasanabilir. \n"
            + "Ancak bu surec, yeni bir baslangic icin gereken temizlik ve arinmayi \n"
            + "temsil eder. Acinizi kabullenmek, duygusal iyilesmenin ilk adimi olacaktir.",
            
            "Is hayatinda bir projeyi ya da mevcut bir durumu sonlandirmak \n"
            + "zorunda kalabilirsiniz. Bu durum baslangicta zor gorunse de, uzun \n"
            + "vadede size yeni firsatlarin kapisini acacaktir. Gecmisi geride birakmak, \n"
            + "ilerlemeniz icin bir zorunluluk haline gelebilir."
        },
        
        //60(Kılıç Prensi)
        {
            "Yeni bilgi arayisi, merak ve zihinsel hareketliligi temsil eder. \n"
            + "Bu kart, ogrenmeye acik oldugunuz ve hayatinizdaki durumlari analiz \n"
            + "etmek icin keskin bir zihinle hareket ettiginiz bir donemi isaret eder. \n"
            + "Ancak bazen fazla merakli davranmak, baskalarinin özel alanina \n"
            + "mudahale etmenize neden olabilir.",
            
            "İliskide partnerinizi daha iyi anlamak ve duygularinizi analiz \n"
            + "etmek icin caba sarf ediyorsunuz. Ancak fazla sorgulayici davranmak \n"
            + "yerine, akista kalmayi ogrenmek iliskiniz icin daha faydali olacaktir. \n"
            + "Bekarlar icin bu kart, bir iliskiye dair merak ve heves dolu bir \n"
            + "donemi temsil eder.",
            
            "Is hayatinda yeni bilgiler edinmek, arastirmalar yapmak ve \n"
            + "zihinsel olarak aktif bir sekilde calismak sizi basariya goturebilir. \n"
            + "Ancak detaylara cok fazla odaklanarak buyuk resmi kacirmamaya dikkat etmelisiniz."
        },
        
        //61(Kılıç Şövalyesi)
        {
            "Bu kart, hizli hareket, cesaret ve kararliligi temsil eder. Hedeflerinize \n"
            + "ulasmak icin tum gucunuzle harekete gectiginiz bir donemdesiniz. \n"
            + "Ancak bu surecte, aceleci davranarak detaylari gozden kacirma riski \n"
            + "tasiyabilirsiniz. Dusunmeden hareket etmekten kacinin ve adimlarinizi \n"
            + "dikkatle planlayin.",
            
            "İliskide heyecanli ve hizli gelismeler yasayabilirsiniz. \n"
            + "Ancak bu durum, bazen sabirsiz davranmaniza ve iliskinizde gerilim \n"
            + "yaratmaniza neden olabilir. Dengeli bir tutum sergileyerek \n"
            + "partnerinizle uyum icinde hareket etmek onemlidir.",
            
            "Is hayatinda hedeflerinize ulasmak icin hizli ve cesur bir \n"
            + "sekilde ilerliyorsunuz. Ancak bu surecte detaylara dikkat etmeli ve \n"
            + "aceleci kararlar almaktan kacinmalisiniz. Stratejik bir yaklasim, \n"
            + "basariya daha emin adimlarla ulasmanizi saglayacaktir."
        },
        
        //62(Kılıç Kraliçesi)
        {
            "Bu kart, mantik, objektiflik ve netligi temsil eder. Bu donem, \n"
            + "duygularinizi bir kenara birakarak olaylara daha analitik bir \n"
            + "gozle bakmaniz gerektigini gosterir. Kararlarinizda durustluk ve \n"
            + "gercekciligi on planda tutarak, hayatinizdaki sorunlari cozebilirsiniz.",
            
            "İliskide netlik ve gercekci bir tutum sergiliyorsunuz. Duygusal \n"
            + "olarak kendinizi daha guclu hissettiginiz bu donemde, iliskinizin dinamiklerini \n"
            + "dogru bir sekilde analiz edebilirsiniz. Bekarlar icin bu kart, \n"
            + "mantikli bir sekilde ilerlenmesi gereken bir iliskiyi isaret eder.",
            
            "Is hayatinda analitik dusunce gucunuzle on plana cikiyorsunuz. \n"
            + "Mantikli kararlar alarak ve stratejik bir sekilde hareket ederek basariya \n"
            + "ulasabilirsiniz. Insanlarla iletisiminizde net ve durust bir yaklasim \n"
            + "sergilemeniz, kariyerinizde size avantaj saglayacaktir."
        },
        
        //63(Kılıç Kralı)
        {
            "Otorite, liderlik ve zihinsel gucun temsilcisidir. Bu kart, olaylara \n"
            + "objektif ve adil bir sekilde yaklasmaniz gerektigini gosterir. \n"
            + "Kararlarinizi mantik cercevesinde alarak, hayatinizda duzen ve kontrol \n"
            + "saglamaniz mumkun olacaktir.",
            
            "İliskide olgunluk ve kararlilikla hareket ettiginiz bir donemdesiniz. \n"
            + "Partnerinizle guclu bir bag kurarak iliskinizi daha saglam bir temele \n"
            + "oturtabilirsiniz. Bekarlar icin bu kart, mantik ve duygular arasinda \n"
            + "denge kurarak dogru bir iliskiyi secmeniz gerektigini ifade eder.",
            
            "Is hayatinda liderlik yeteneklerinizle on plana cikiyorsunuz. \n"
            + "Mantikli, stratejik ve adil bir yaklasimla kariyerinizde onemli basarilara \n"
            + "imza atabilirsiniz. Zihinsel gucunuz ve kararliliginiz, sizi her turlu \n"
            + "zorlugun ustesinden getirebilecek bir noktaya tasiyacaktir."
        },
        
        //64(Değnek Ası)
        {
            "Bu kart, yaraticilik, enerji ve yeni baslangiclari simgeler. \n"
            + "Hayatiniza taze bir enerji girebilir, yeni projeler ve fikirler gelistirmek \n"
            + "icin hevesli hissedebilirsiniz. Bu kart, motivasyonunuzun yuksek oldugu \n"
            + "ve harekete gecmek icin dogru bir zamanda oldugunuzu gosterir. Yaraticilik \n"
            + "ve tutku dolu bir donemdesiniz; bu enerjiyi iyi degerlendirirseniz, \n"
            + "buyuk basarilar elde edebilirsiniz.",
            
            "Ask hayatinizda heyecan verici bir baslangic ya da tutkuyu yeniden \n"
            + "kesfetme zamani olabilir. Mevcut iliskinizde tutkuyu artiracak yeni bir \n"
            + "doneme giriyor olabilirsiniz. Bekarlar icin, yeni ve heyecan verici bir \n"
            + "iliski olasiligi oldukca yuksektir. Bu kisi, size enerji ve cosku katabilir.",
            
            "Is hayatinda yaratici bir donemdesiniz ve yeni projelere baslamak \n"
            + "icin ideal bir zamandasiniz. Bu kart, enerjinizin yuksek oldugunu ve \n"
            + "kariyerinizde cesur adimlar atmak icin ilham aldiginizi ggsterir. Is \n"
            + "fikirlerinizi uygulamaya gecirmek icin mukemmel bir donemdesiniz."
        },
        
        //65(Değnek İkilisi)
        {
            "Bu kart, planlama ve gelecekteki firsatlari degerlendirme surecini \n"
            + "isaret eder. Su anda elinizde guclu secenekler olabilir ve hangisinin \n"
            + "sizin icin daha iyi sonuclar doguracagini degerlendirme asamasinda olabilirsiniz. \n"
            + "Gelecekteki basarilar icin stratejik dusunme zamani. Risk almak zorunda \n"
            + "kalabilirsiniz, ancak dikkatli bir planlama ile buyuk kazanclar elde etmeniz mumkun.",
            
            "Ask hayatinizda bir karar verme surecindesiniz. Mevcut iliskinizin \n"
            + "gelecegi hakkinda dusunceleriniz olabilir veya yeni bir iliskiye \n"
            + "baslamak konusunda tereddut yasiyor olabilirsiniz. Bu kart, duygusal \n"
            + "olarak ileriye donuk planlar yapmaniz gerektigini isaret eder. \n"
            + "Bekarlar icin, olasi iki farklı secenek arasında kalabilirsiniz.",
            
            "ıs hayatinda kararlar ve stratejik planlar yapma zamani. \n"
            + "Hangi yone ilerleyeceginize karar vermeniz gerekebilir. Yeni bir projeye \n"
            + "baslamak ya da mevcut isinizi buyutmek gibi sesenekler onunuze gelebilir. \n"
            + "Bu surecte sabirli ve dikkatli olursaniz, basari sizin icin kacinilmazdir."
        },
        
        //66(Değnek Üçlüsü)
        {
            "Bu kart, ilerleme ve buyumeyi temsil eder. Daha onceki cabalarinizin \n"
            + "sonuclarini gormeye baslayabilir ve gelecekteki adimlarinizi planlamaya \n"
            + "devam edebilirsiniz. Bu kart, genis ufuklar ve yeni firsatlar anlamina gelir. \n"
            + "Hayatinizda onemli bir yolculuga cikabilir ya da yeni bir maceraya atilabilirsiniz.",
            
            "Ask hayatinizda yeni ufuklara yelken acma zamani. Mevcut iliskinizde \n"
            + "bir sonraki asamaya gecebilir veya partnerinizle birlikte buyuk planlar \n"
            + "yapabilirsiniz. Bekarlar icin, uzak mesafeli bir iliski ya da seyahat \n"
            + "sirasinda yeni biriyle tanisma olasiligi vardir. Bu kart, ask hayatinizda \n"
            + "hareket ve heyecani isaret eder.",
            
            "Is hayatinda, cabalarinizin sonuclarini gormeye basladiginiz bir \n"
            + "doneme girdiniz. Kariyerinizde buyume ve genisleme firsatlari karsiniza \n"
            + "cikabilir. Yeni projeler ya da uluslararasi baglantilar kurma \n"
            + "olasiligi vardir. Bu surecte cesur ve kararli olursaniz, buyuk \n"
            + "bacarilar elde edebilirsiniz."
        },
        
        //67(Değnek Dörtlüsü)
        {
            "Bu kart, kutlama, huzur ve istikrar anlamina gelir. Bu kart, \n"
            + "hayatinizdaki olumlu gelismeleri kutlamak icin bir firsat oldugunu \n"
            + "gosterir. Bir hedefe ulasmis veya bir donemi basariyla tamamlamis \n"
            + "olabilirsiniz. Aile, arkadaslar ve sevdiklerinizle birlikte huzur \n"
            + "dolu bir donemdesiniz.",
            
            "İliskilerde mutluluk ve kutlama zamani. Partnerinizle iliskinizde \n"
            + "bir donum noktasina ulasmis ve birlikte kutlama yapabilirsiniz. Bu kart, \n"
            + "evlilik, nisan ya da iliskiyi bir sonraki asamaya tasima gibi olaylari \n"
            + "simgeler. Beksrlar icin, ask hayatinizda ciddi ve guvenilir bir \n"
            + "iliskiye adim atma olasiligi yuksektir.",
            
            "Is hayatinda basarilarinizi kutlama zamani. Uzun suredir \n"
            + "uzerinde calistiginiz bir projeyi tamamlamis veya onemli bir hedefe \n"
            + "ulasmis olabilirsiniz. Bu kart, is arkadaslariniz ve cevrenizle birlikte \n"
            + "basarinizi kutlamaniz gerektigini gosterir. Ayni zamanda, kariyerinizde \n"
            + "guvenli ve saglam bir temele ulastiginizi da simgeler."
        },
        
        //68(Değnek Beşlisi)
        {
            "Bu kart, rekabet, catisma ve farkli gorusleri temsil eder. \n"
            + "Hayatinizda bir kaos ya da mucadele donemi olabilir, ancak bu zorluklar, \n"
            + "buyume ve gelisme icin bir firsattir. Catismalari cozmek ve uyum \n"
            + "saglamak icin esnek bir tutum sergilemeniz gerekebilir.",
            
            "İliskilerde anlasmazliklar ve kucuk çatismalar yasanabilir. \n"
            + "Partnerinizle iletisime odaklanarak bu sorunlarin ustesinden gelebilirsiniz. \n"
            + "Bekarlar icin, birden fazla kisinin ilgisiyle karsilasabilirsiniz, \n"
            + "bu da bir karar verme surecine neden olabilir.",
            
            "Is hayatinda rekabetci bir ortamdasiniz. Cevrenizdekilerle \n"
            + "catismalar ya da fikir ayriliklari yasanabilir, ancak bu surecte kararli \n"
            + "ve yapici bir tutum sergilerseniz, kendinizi kanitlayabilirsiniz. \n"
            + "Bu kart, zorluklarla basa cikmanin kariyeriniz icin faydali olacagini gosterir."
        },
        
        //69(Değnek Altılısı)
        {
            "Bu kart, zafer, taninma ve basariyi simgeler. Uzun suredir uzerinde \n"
            + "calistiginiz bir hedefe ulastiginiz veya baskalari tarafindan takdir \n"
            + "edildiginiz bir doneme isaret eder. Cabalarinizin karsiligini aliyorsunuz \n"
            + "ve hayatinizda pozitif bir donum noktasi yasaniyor. Bu basari, size \n"
            + "daha fazla motivasyon ve ozguven kazandirabilir.",
            
            "Ask hayatinizda mutluluk ve basariya ulastiginiz bir doneme girdiniz. \n"
            + "Partnerinizle iliskinizin olumlu yonde ilerledigini hissedebilir ve \n"
            + "sevginizin karsilikli olarak buyudugunu gorebilirsiniz. Bekarlar icin, \n"
            + "cevrenizde size hayran olan bir kisi fark edilebilir ve bu \n"
            + "kisiyle mutlu bir baslangic yapabilirsiniz.",
            
            "Is hayatinda taninma ve basari zamani. Cabalarinizin sonucunda \n"
            + "bir terfi, odul veya onemli bir proje tamamlanabilir. Bu kart, \n"
            + "liderlik vasiflarinizin fark edilmesi ve cevrenizden destek gormeniz \n"
            + "anlamina gelir. Is hayatinizda parlak bir donemdesiniz; bu \n"
            + "firsatlari iyi degerlendirin."
        },
        
        //70(Değnek Yedilisi)
        {
            "Bu kart, mucadele, savunma ve kendi durusunuzu koruma gerekliligini \n"
            + "isaret eder. Zorluklarla karsi karsiya olabilirsiniz, ancak kararli \n"
            + "bir sekilde hedeflerinizi savunmaniz gerekiyor. Baskalarinin sizin \n"
            + "uzerinizde baski kurmaya calısabilecegi bir donemde, kendi \n"
            + "inanslariniza sadik kalarak yol almaniz onemlidir.",
            
            "İliskinizde dis etkenlerden kaynaklanan baskilarla karsilasabilirsiniz. \n"
            + "Partnerinizle aranizda guclu bir bag kurarak bu baskilara karsi \n"
            + "dayanikli olmaniz gerekiyor. Bekarlar icin, duygularinizin ve \n"
            + "degerlerinizin test edildigi bir surec olabilir. Sabirli ve kararli olun.",
            
            "Is hayatinda rekabet ve baski ile karsilasabilirsiniz. \n"
            + "Cevrenizdekiler sizin basarilariniza goz dikebilir veya sizin pozisyonunuzu \n"
            + "sorgulayabilir. Bu surecte guclu bir durus sergileyerek basariya \n"
            + "ulasabilirsiniz. Kendinizi kanitlamak ve hak ettiginiz yeri korumak \n"
            + "icin caba sarf etmelisiniz."
        },
            
        //71(Değnek Sekizlisi)
        {
            "Bu kart, hiz, hareket ve ilerleme anlamina gelir. Hayatinizda \n"
            + "hizli gelismelerin yasanacagi bir doneme girdiginizi isaret eder. \n"
            + "Beklenmedik haberler alabilir veya ani kararlar vermek zorunda kalabilirsiniz. \n"
            + "Bu surecte enerjinizi iyi yonlendirerek firsatlari degerlendirmeniz onemlidir.",
            
            "Ask hayatinizda hizli ve heyecan verici gelismeler yasanabilir. \n"
            + "Partnerinizle iliskinizde bir anda yogun bir bag hissedebilir veya bir \n"
            + "sonraki asamaya gecebilirsiniz. Bekarlar icin, yeni bir kisiyle \n"
            + "tanisma veya ani bir duygusal bag kurma olasiligi vardir.",
            
            "Is hayatinda hizli bir ilerleme donemi. Beklediginiz projeler \n"
            + "hizla sonuclanabilir veya yeni firsatlar aniden karsınıza cikabilir. \n"
            + "Bu kart, harekete gecme ve hizli kararlar alma zamani oldugunu \n"
            + "gosterir. Enerjinizi odaklayarak bu firsatlari en iyi sekilde \n"
            + "degerlendirin."
        },
        
        //72(Değnek Dokuzlusu)
        {
            "Bu kart, direnc, dayaniklilik ve son bir cabanin gerektigi bir \n"
            + "donemi simgeler. Zorlu bir surecten gecmis olabilirsiniz, ancak pes \n"
            + "etmeden mucadeleye devam etmeniz onemlidir. Bu kart, bir hedefe cok \n"
            + "yaklastiginizi ve biraz daha dayanmaniz gerektigini isaret eder.",
            
            "İliskinizde gecmiste yasanan zorluklar sizi yipratmis olabilir, ancak \n"
            + "pes etmeden iliskiyi onarma cabalariniz devam ediyor. Partnerinizle \n"
            + "birlikte sorunlarin ustesinden gelmek icin son bir caba harcamaniz gerekebilir. \n"
            + "Bekarlar icin, gecmisteki hayal kirikliklarinin sizi engellemesine izin vermeden \n"
            + "yeni bir iliskiye acik olmaniz onemlidir.",
            
            "Is hayatinda yogun ve yorucu bir surecten geciyor olabilirsiniz. \n"
            + "Ancak bu kart, hedefinize cok yaklastiginizi ve biraz daha dayanmaniz gerektigini \n"
            + "gosterir. Cabalarinizin meyvelerini almak icin motivasyonunuzu \n"
            + "koruyun ve yilmadan devam edin."
        },
        
        //73(Değnek Onlusu)
        {
            "Bu kart, agir yukler, sorumluluklar ve bitisleri temsil eder. \n"
            + "Hayatinizda asiri yuklenmis hissedebilir veya cok fazla sorumluluk \n"
            + "aldiginiz bir donemde olabilirsiniz. Bu durum, sizi duygusal ve \n"
            + "fiziksel olarak yipratabilir; bu nedenle destek aramak ve yukunuzu \n"
            + "hafifletmek onemlidir.",
            
            "İliskinizde fazla sorumluluk almis ve bu durumun sizi yormus olabilecegi \n"
            + "bir donemde olabilirsiniz. Partnerinizle acik bir iletisim kurarak \n"
            + "bu yuku paylasmaniz gerekebilir. Bekarlar icin, duygusal gecmisinizin \n"
            + "yuku yeni iliskilere acik olmanizi zorlastirabilir; gecmisi geride \n"
            + "birakmaya calismalisiniz.",
            
            "Is hayatinda uzerinize cok fazla yuk almis olabilirsiniz. \n"
            + "Bu kart, asiri sorumluluklarin sizi yordugunu ve yardima ihtiyac \n"
            + "duydugunuzu gosterir. Daha verimli calismak ve yukunuzu hafifletmek \n"
            + "icin gorevlerinizi paylasmayi ogrenmeniz gerekebilir."
        },
        
        //74(Değnek Prensi)
        {
            "Bu kart, merak, macera ve yeni baslangiclari temsil eder. Bu \n"
            + "kart, hayatiniza yenilik katma, kesfetme ve yeni fikirlere acik olma \n"
            + "zamaninin geldigini isaret eder. Kendinizi yeni bir projeye, hobiye \n"
            + "veya yolculuga baslamak icin motive hissedebilirsiniz. Bu kart, ayni \n"
            + "zamanda genc ve enerjik bir ruh hali ile dunyayı kesfetme arzusunu simgeler. \n"
            + "Hayatinizda yaratici bir doneme girebilirsiniz; fikirlerinizi hayata \n"
            + "gecirmek icin cesaret ve tutkuya sahipsiniz.",
            
            "Ask hayatinizda macera dolu ve heyecan verici bir donemdesiniz. \n"
            + "Mevcut iliskinizde yeni bir seyler deneme ya da partnerinizle iliskinizi \n"
            + "canlandirma arzusu hissedebilirsiniz. Bekarlar icin, hayatiniza enerji \n"
            + "ve nese getirecek biriyle tanisma olasiligi yuksektir. Bu kisi, sizi yeni \n"
            + "seyler kesfetmeye tesvik eden biri olabilir.",
            
            "Is hayatinizda yenilik ve yaraticilik on planda. Yeni bir proje, \n"
            + "is firsati ya da ogrenme deneyimi sizi bekliyor olabilir. Bu kart, aynı \n"
            + "zamanda kariyerinizde yaratici dusuncelerinizle fark yaratabileceginizi \n"
            + "ve enerjinizle cevrenize ilham verebileceginizi gosterir. Ancak bu surecte \n"
            + "fikirlerinizi somut hale getirmek icin planli bir sekilde hareket etmelisiniz."
        },
        
        //75(Değnek Şövalyesi)
        {
            "Bu kart, cesaret, tutku ve hareketi simgeler. Bu kart, hayatinizda \n"
            + "enerjik ve heyecan verici bir doneme girdiginizi isaret eder. Su anda \n"
            + "hedeflerinize ulasmak icin cesur adimlar atmaya hazir hissediyorsunuz. \n"
            + "Risk alarak hayallerinize dogru ilerleyebilir, yeni maceralara atilabilirsiniz. \n"
            + "Ancak bu surecte sabirsizlik ve dikkatsizlikten kacinmaniz onemlidir. \n"
            + "Hizli dusunme ve ani kararlar, bazen beklenmedik sonuclar dogurabilir.",
            
            "Ask hayatinizda tutkulu ve heyecan verici bir donemdesiniz. Partnerinizle \n"
            + "iliskinizde enerjik bir bag hissedebilir ve birlikte yeni maceralara atilma \n"
            + "istegi duyabilirsiniz. Bekarlar icin, karizmatik ve dinamik bir kisiyle \n"
            + "karsilasma ihtimali vardir. Ancak iliskinizin hizla gelismesi, bazen \n"
            + "istikrarli bir temel olusturmayi zorlastirabilir, bu nedenle sabirli olmalisiniz.",
            
            "Is hayatinizda buyuk bir motivasyon ve enerjiyle hareket ediyorsunuz. \n"
            + "Yeni projelere baslamak icin hevesli olabilir ve cesur adimlar atabilirsiniz. \n"
            + "Ancak bu surecte aceleci davranmamaya ozen gostermelisiniz. Hedeflerinize \n"
            + "kararli bir sekilde ilerlerken, detaylara dikkat etmek ve sabirli olmak \n"
            + "basariyi garantileyecektir."
        },
        
        //76(Değnek Kraliçesi)
        {
            "Bu kart, karizma, guven ve ilham kaynagi olmayı temsil eder. \n"
            + "Bu kart, kendinize olan guveninizin arttigini ve cevrenize enerji ve \n"
            + "ilham yaydiginiz bir donemde oldugunuzu isaret eder. Yarativi \n"
            + "projelerde liderlik edebilir ve baskalarini cesaretlendirebilirsiniz. \n"
            + "Hayatinizda sicaklik, nese ve tutkunun on planda oldugu bir donemdesiniz.",
            
            "Ask hayatinizda tutkulu ve enerji dolu bir donemdesiniz. Partnerinizle \n"
            + "aranizdaki bagin daha da guclendigini ve iliskinizde daha fazla heyecan \n"
            + "oldugunu hissedebilirsiniz. Bekarlar icin, kendine guvenen ve cekici bir \n"
            + "kisiyle tanisma olasiligi vardir. Bu kisi, sizin icin ilham kaynagi olabilir.",
            
            "Is hayatinizda liderlik becerileriniz on planda. Projelerde baskalarina \n"
            + "ilham veriyor ve cevrenizdekilere guclu bir rehberlik sagliyorsunuz. Bu kart, \n"
            + "karizmaniz ve enerjinizle buyuk basarilar elde edeceginiz bir donemi isaret eder. \n"
            + "Yeni firsatlari degerlendirin ve cesur adimlar atmaktan cekinmeyin."
        },
        
        //77(Değnek Kralı)
        {
            "Bu kart, liderlik, guc ve kararliligi temsil eder. Hayatinizda \n"
            + "hedeflerinizi net bir sekilde belirlediginiz ve bu hedeflere ulasmak icin guclu \n"
            + "bir iradeyle ilerlediginiz bir donemdesiniz. Bu kart, hem kisisel hem de \n"
            + "profesyonel hayatinizda kararlilikla ilerlemenizi ve diger insanlara ilham \n"
            + "vermenizi isaret eder. Guclu bir liderlik donemi yasayabilirsiniz.",
            
            "İliskinizde guclu bir bag ve guven on plandadir. Partnerinizle birlikte \n"
            + "saglam ve istikrarli bir iliski kurmus olabilirsiniz. Bu kart, iliskinizin \n"
            + "sorumluluklar ve sevgiyle buyudugunu gosterir. Bekarlar icin, guclu, karizmatik \n"
            + "ve guvenilir bir partnerle tanisma olasiligi yuksektir. Bu kisi, \n"
            + "size hem ilham hem de destek saglayabilir.",
            
            "Is hayatinizda liderlik ve basari donemi. Cevrenizdeki \n"
            + "insanlara rehberlik ediyor ve kararliliginizla projeleri basariya \n"
            + "ulastiriyorsunuz. Bu kart, buyuk hedefler belirlediginizi ve bu hedeflere \n"
            + "ulasmak icin gereken enerjiyi ve stratejiyi uyguladiginizi gosterir. \n"
            + "Ayrica, bu donemde yeni firsatlar ve buyuk basarilar elde etme \n"
            + "sansiniz oldukca yuksektir."
        }
    };         
}


import java.util.Scanner;

public class Okuma {
    
    public void kartCekVeYorumYazdir() {
        
        Scanner klavye = new Scanner(System.in);

        // Kullanıcıdan yorum türü seçmesini iste
        System.out.println("Bir yorum turu seciniz: ");
        System.out.println("1 - Genel Yorum");
        System.out.println("2 - Ask Yorumu");
        System.out.println("3 - Kariyer Yorumu");
        System.out.print("Seciminiz: ");
        int secim = klavye.nextInt();

        // Major ve Minor Arcana kartlarını birleştir
        
        String[] tumKartlar = new String[MajorArcana.majorKartlar.length + MinorArcana.minorKartlar.length];
        System.arraycopy(MajorArcana.majorKartlar, 0, tumKartlar, 0, MajorArcana.majorKartlar.length);
        System.arraycopy(MinorArcana.minorKartlar, 0, tumKartlar, MajorArcana.majorKartlar.length, MinorArcana.minorKartlar.length);

        // Major ve Minor anlamlar dizilerini birleştir
        
        String[][] tumAnlamlar = new String[MajorArcana.anlamlar.length + MinorArcana.kAnlamlar.length][];
        System.arraycopy(MajorArcana.anlamlar, 0, tumAnlamlar, 0, MajorArcana.anlamlar.length);
        System.arraycopy(MinorArcana.kAnlamlar, 0, tumAnlamlar, MajorArcana.anlamlar.length, MinorArcana.kAnlamlar.length);

        // Random bir kart seç (Math.random() kullanarak)
        
        int rastgeleKartIndex = (int) (Math.random() * tumKartlar.length);
        String secilenKart = tumKartlar[rastgeleKartIndex];
        String[] secilenAnlamlar = tumAnlamlar[rastgeleKartIndex];

        // Seçilen yorumu ekrana yazdır
        
        System.out.println("\nSecilen Kart: " + secilenKart);
        switch (secim) {
            case 1:
                System.out.println("Genel Yorum: ");
                System.out.println(secilenAnlamlar[0]);
                break;
            case 2:
                System.out.println("Ask Yorumu: ");
                System.out.println(secilenAnlamlar[1]);
                break;
            case 3:
                System.out.println("Kariyer Yorumu: ");
                System.out.println(secilenAnlamlar[2]);
                break;
            default:
                System.out.println("Gecersiz secim! Lütfen 1, 2 veya 3'ü seciniz.");
                break;
        }

        klavye.close();
    }
}


import java.util.Scanner;

public class Main {
    
    public static void main(String[] args){
        
        Okuma okuma = new Okuma();
        
        okuma.kartCekVeYorumYazdir();
    }
}


public abstract class Burc {

    protected String name;
    protected String [] anlamlar;
    
    protected static String[] burclar = {"Koc", "Boga", "Ikizler", "Yengec", "Aslan","Basak","Terazi","Akrep","Yay","Oglak","Kova","Balik"};
    
    public Burc (String name){
        
        this.name=name;
        
    }
    
    public String getName(){
        
        return this.name;
    }
    
    public abstract String[] getAnlamlar();
    
    public String toString(){
        
        return ("Burc Ismi: "+name);
    }
}


public class AylikBurc extends Burc{
    
    public AylikBurc(String name) {
        super(name);
    }
    
    @Override
    public String[] getAnlamlar() {
        return aylikAnlamlar;
    }
    
    protected static String[] aylikAnlamlar={
      
        //Koç
         
             "Genel Bakis: Ocak ayi Koc burclari icin hareketli bir baslangic vadediyor. \n"
             + "Kariyer, iliskiler ve kisisel hedeflerinizde onemli adimlar \n"
             + "atabileceginiz bu donemde, enerjinizi dogru yonlendirmeniz basariyi getirecek.\n\n"
             
             + "Kariyer: Ayin basinda Gunes’in Oglak burcundaki konumu kariyerinize ve toplumsal \n"
             + "statunuze odaklanmanizi sagliyor. Is yerinde artan sorumluluklar ve dikkat \n"
             + "gerektiren projeler gundemde olacak. Eger is degisikligi dusunuyorsaniz, \n"
             + "19 Ocak’tan itibaren Merkur’un duz hareketine gecmesiyle daha net kararlar \n"
             + "alabilirsiniz. Ozellikle ayin son haftasinda somut adimlar atarak kariyerinizde \n"
             + "kalici baaarilar elde edebilirsiniz.\n\n"
             
             + "Ask ve Iliskiler: 10 Ocak’a kadar Venus’un Yay burcundaki etkisi, iliskilerde \n"
             + "ozgurluk ve eglence arayisini artiriyor. Partnerinizle macera dolu bir tatil \n"
             + "veya keyifli planlar yapabilirsiniz. Yalnizsaniz, bu donemde cesur ve farkli \n"
             + "bir insanla tanisma ihtimaliniz yuksek. 25 Ocak’tan sonra duygusal derinlik \n"
             + "ve baglilik ihtiyaciniz artabilir.\n\n"
             
             + "Saglik: Yogun is temposu nedeniyle dinlenmeye zaman ayirmaniz onemli. Stresi azaltmak \n"
             + "icin spor veya meditasyon gibi aktivitelerden faydalanabilirsiniz. Bagisiklik sisteminizi \n"
             + "desteklemek icin saglikli bir beslenme plani olusturun.\n\n"
             
             + "Onemli Tarihler:\n"
             + "6 Ocak: Yengec burcundaki Dolunay, ailevi meseleleri gundeme getiriyor. Evle ilgili \n"
             + "bir degisiklik planlayabilirsiniz.\n" 
             + "31 Ocak: Oglak burcundaki Yeni Ay, is hayatinizda yeni bir baslangic yapma firsati sunuyor.",
         
         
         //Boğa
         
             "Genel Bakis: Boga burclari icin Ocak ayi, hem icsel dengeyi saglamaya hem de finansal konularda \n"
             + "planli ilerlemeye odaklanacaklari bir donem. Iliskilerde sabir ve guven on planda olacak.\n\n"
             
             + "Kariyer: Ayin basinda Gunes’in Oglak burcundaki konumu, uzun vadeli planlar yapmaniz icin harika \n"
             + "bir firsat sunuyor. Disiplinli bir sekilde calisarak projelerinizi basariyla tamamlayabilirsiniz. \n"
             + "Ozellikle egitim veya yurt disi baglantili islerde sansli bir donemdesiniz. 19 Ocak’tan sonra \n"
             + "iletisim trafigi artabilir ve bekleyen isleriniz hiz kazanabilir.\n\n"
             
             + "Ask ve Iliskiler: Venus, Ocak ayinin ilk yarisinda Yay burcunda ilerlerken, iliskilerde spontane \n"
             + "ve neseli bir enerji hakim. Partnerinizle daha acik ve samimi bir iletisim kurabilirsiniz. Yalnizsaniz, \n"
             + "bu donemde hayatiniza girecek biriyle macera dolu bir baslangic yapabilirsiniz. Ayin son haftasinda \n"
             + "iliskilerde daha ciddi ve uzun vadeli bir yaklasim sergileyebilirsiniz.\n\n"
             
             + "Saglik: Ruhsal ve fiziksel sagliginiza odaklanmaniz gereken bir donem. Is yukunuz artabilir; \n"
             + "bu nedenle duzenli egzersiz ve dinlenmeye ozen gostermelisiniz. Saglikli beslenme \n"
             + "aliskanliklarinizi gozden gecirmek faydali olacaktir.\n\n"
             
             + "Onemli Tarihler:\n"
             + "15 Ocak: Ikizler Dolunayi, finansal konularda netlesme saglayabilir.\n" 
             + "31 Ocak: Yeni Ay, is hayatinizda onemli bir donum noktasi olabilir.",
         
         
         //İkizler
         
             "Genel Bakis: Ocak ayi, Ikizler burclari icin yenilikler ve iletisim firsatlariyla dolu olacak. \n"
             + "Hem kariyer hem de sosyal cevrenizdeki hareketlilik, size yeni kapilar acabilir.\n\n"
             
             + "Kariyer: Merkur retrosunun sona ermesiyle, islerinizde bekleyen projelerinizi tamamlamak \n"
             + "ve yeni girisimlerde bulunmak icin mukemmel bir doneme giriyorsunuz. Yaratici fikirleriniz \n"
             + "ve pratik zekaniz sayesinde is hayatinizda fark yaratabilirsiniz. Ozellikle \n"
             + "ekip calismalarinda liderlik rolu ustlenebilirsiniz.\n\n"
             
             + "Ask ve Iliskiler: Venus’un etkisiyle Ocak ayinin ilk yarisinda romantik ve heyecanli \n"
             + "bir enerji hakim olacak. Partnerinizle birlikte kisa seyahatler veya romantik organizasyonlar \n"
             + "planlayabilirsiniz. Yalnizsanız, sosyal cevrenizde dikkat ceken biriyle tanisabilirsiniz.\n\n"
             
             + "Saglik: Zihinsel yorgunlugu azaltmak icin meditasyon veya yoga gibi aktivitelerden faydalanabilirsiniz. \n"
             + "Duzenli uyku ve saglikli beslenme rutini, enerjinizi yuksek tutmaniza yardimci olacaktir.\n\n"
             
             + "Onemli Tarihler:\n"
             + "6 Ocak: Dolunay, ozel hayatinizda netlesmesi gereken konulari gundeme getirebilir.\n" 
             + "20 Ocak: Sosyal cevrenizde yeni baglantilar kurabilirsiniz.",
         
         
         //Yengeç
         
             "Genel Bakis: Ocak, Yengec burclari icin ailevi meseleler, duygusal baglar ve \n"
             + "kariyer odakli bir ay olacak. Kendi ihtiyaclarinizla cevrenizdekilerin \n"
             + "beklentileri arasinda denge kurmaya calisabilirsiniz.\n\n"
             
             + "Kariyer: Gunes’in Oglak burcundaki konumu, kariyerinizde uzun vadeli hedeflere \n"
             + "yonelmenizi destekliyor. Bu donemde sabirli ve kararli bir sekilde ilerlemek onemlidir. \n"
             + "Ozellikle 19 Ocak’tan itibaren is arkadaslarinizla olan iletisimde iyilesmeler yasanabilir \n"
             + "ve bekleyen projelerde ilerleme saglayabilirsiniz. Ay sonuna dogru finansal bir artis \n"
             + "veya kariyerinizde yukselme sansi dogabilir.\n\n"
             
             + "Ask ve Iliskiler: Ocak ayinin ilk haftasinda Dolunay, ailevi konulari gundeme getirebilir. \n"
             + "Partnerinizle iliskinizde destekleyici bir donem gecirebilir, birlikte gecmis meseleleri \n"
             + "cozebilirsiniz. Eger bir iliskiniz yoksa, guven ve baglilik arayisiniz bu ay on planda olacak.\n\n"
             
             + "Saglik: Duygusal hassasiyetiniz bu ay artabilir, bu yuzden ruhsal sagliginiza dikkat etmeniz \n"
             + "onemli. Yoga, meditasyon veya doga yuyuyusleriyle kendinizi rahatlatabilirsiniz.\n\n"
             
             + "Onemli Tarihler:\n"
             + "6 Ocak: Yengec burcundaki Dolunay, ailevi ve duygusal meselelerde netlesme saglayabilir.\n" 
             + "31 Ocak: Yeni Ay, kariyerinizde yeni bir sayfa acma firsati sunuyor.",
         
         
         //Aslan
         
             "Genel Bakis: Ocak ayi Aslan burclari icin yaraticiliginizi ve liderlik yeteneklerinizi \n"
             + "sergilemek icin harika bir zaman. Hem sosyal cevreniz hem de kariyer hedefleriniz \n"
             + "acisindan guclu bir donemdesiniz.\n\n"
             
             + "Kariyer: Ayin basinda, is hayatinizda sorumluluklarinizi artırabilir ve daha fazla \n"
             + "gorunurluk kazanabilirsiniz. Yaraticiliginizi islerinize yansitarak fark yaratabilirsiniz. \n"
             + "Ozellikle 19 Ocak’tan itibaren iletisim ve is birliklerinde buyuk bir akicilik yasanacak. \n"
             + "Ay sonuna dogru, buyuk bir proje veya terfi haberi alabilirsiniz.\n\n"
             
             + "Ask ve Iliskiler: Ocak ayinin ilk yarisinda, Venus’un enerjisiyle ask hayatinizda heyecan ve \n"
             + "romantizm artiyor. Partnerinizle aranizdaki uyum guclenebilir. Eger bir iliskiniz yoksa, \n"
             + "bu donemde cekici bir enerjiniz olacak ve dikkatleri uzerinize cekebilirsiniz.\n\n"
             
             + "Saglik: Enerjik bir ay gecireceksiniz, ancak dinlenmeyi ihmal etmemeniz onemli. \n"
             + "Duzenli egzersiz yaparak fiziksel gucunuzu artirabilirsiniz.\n\n"
             
             + "Onemli Tarihler:\n"
             + "20 Ocak: Gunes’in Kova burcuna gecisi, iliskilerinizde ve sosyal cevrenizde hareketlilik yaratacak.\n" 
             + "31 Ocak: Yeni Ay, kariyer hedeflerinizi yeniden sekillendirme firsati sunuyor.",
             
         //Başak
             
             "Genel Bakis: Basak burclari icin Ocak, planlama, uretkenlik ve uzun vadeli hedeflere \n"
            + "odaklanma donemi. Ozellikle is hayatinda onemli firsatlar karsiniza cikabilir.\n\n"
            
            + "Kariyer: Gunes’in Oğlak burcundaki konumu, disiplinli calismanizi ve projelerinizi \n"
            + "basariyla tamamlamanizi destekliyor. Is yerinde detayci ve titiz yapiniz sayesinde \n"
            + "takdir toplayabilirsiniz. 19 Ocak’tan itibaren iletisim becerilerinizin artmasiyla, \n"
            + "is gorusmeleri veya ekip calismalari daha verimli hale gelebilir.\n\n"
            
            + "Ask ve Iliskiler: İliskilerde bu ay partnerinizle uyumu artirabilir, duygusal baglarinizi \n"
            + "guclendirebilirsiniz. Yalnizsaniz, ciddi ve mantikli bir iliskiye baslama sansi dogabilir. \n"
            + "Ay sonuna dogru romantik surprizler yasayabilirsiniz.\n\n"
            
            + "Saglik: Yogun tempodan dolayi enerji seviyenizi yuksek tutmaya ozen gosterin. \n"
            + "Saglikli beslenme ve duzenli egzersiz bu donemde size cok iyi gelecek.\n\n"
            
            + "Onemli Tarihler:\n"
            + "6 Ocak: Yengec Dolunayi, sosyal cevrenizde yeni baglantilar kurmaniza yardimci olabilir.\n" 
            + "31 Ocak: Yeni Ay, yaratici projelere baslama sansi sunuyor.",
             
         //Terazi
             
             "Genel Bakis: Ocak, Terazi burclari icin iliskilere ve kisisel hedeflere \n"
            + "odaklanacaklari bir ay olacak. Hayatiniza yeni bir denge getirme firsati dogabilir.\n\n"
            
            + "Kariyer: Kariyerinizde is birlikleri ve ekip calismalari onem kazanacak. \n"
            + "Ayin basinda sorumluluklarinizi gozden gecirebilir ve daha verimli calisma \n"
            + "yollari bulabilirsiniz. 19 Ocak’tan itibaren Merkur’un duz hareketine \n"
            + "gecmesiyle is hayatinizda bekleyen isleriniz hiz kazanabilir.\n\n"
            
            + "Ask ve Iliskiler: Venus’un etkisiyle iliskilerinizde romantizm ve uyum artiyor. \n"
            + "Partnerinizle birlikte duygusal bir bag kurabilirsiniz. Yalnizsaniz, sosyal \n"
            + "cevrenizden biriyle iliski baslatma ihtimaliniz yuksek.\n\n"
            
            + "Saglik: Ruhsal ve fiziksel dengenizi saglamak icin kendinize vakit \n"
            + "ayirmalisiniz. Yoga veya meditasyon bu ay size cok iyi gelecek.\n\n"
            
            + "Onemli Tarihler:\n"
            + "6 Ocak: Dolunay, ozel hayatinizda netlesmesi gereken konulari ortaya cikarabilir.\n" 
            + "20 Ocak: Yeni bir sosyal cevreye girme sansi dogabilir.",
             
         //Akrep
             
             "Genel Bakis: Ocak ayi Akrep burclari icin donusum ve yeniliklerle dolu olacak. \n"
            + "Hem kariyer hem de iliskilerde ciddi adimlar atabileceginiz bir donemdesiniz.\n\n"
            
            + "Kariyer: Gunes’in Oglak burcundaki konumu, is hayatinizda uzun vadeli projelere \n"
            + "odaklanmanizi tesvik ediyor. Ayin ilk yarisinda, detaylara onem vererek basari elde \n"
            + "edebilirsiniz. 19 Ocak’tan itibaren iletisimdeki engeller kalkiyor ve is gorusmeleri \n"
            + "hiz kazaniyor. Ozellikle ay sonunda buyuk bir sorumlulugunuzun odulunu alabilirsiniz.\n\n"
            
            + "Ask ve Iliskiler: İliskilerinizde derinlesme zamani. Partnerinizle duygusal baginizi \n"
            + "guclendirebilir ve gecmis meseleleri cozebilirsiniz. Yalnizsaniz, gizemli ve etkileyici \n"
            + "biriyle tanisabilirsiniz. Venus’un destegiyle romantizm dolu bir donem gecireceksiniz.\n\n"
            
            + "Saglik: Enerjinizi dogru kullanmaya ozen gosterin. Meditasyon ve nefes egzersizleri \n"
            + "ruhsal olarak sizi rahatlatabilir. Uyku duzeninize dikkat etmeniz onemli.\n\n"
            
            + "Onemli Tarihler:\n"
            + "6 Ocak: Dolunay, egitim veya yurt disi baglantili konularda netlesme saglayabilir.\n" 
            + "31 Ocak: Yeni Ay, kariyerinizde yeni bir baslangic yapma firsati sunuyor.",
             
         //Yay
             
             "Genel Bakis: Ocak ayi Yay burclari icin ozgurluk, yaraticilik ve yeni kesiflerle \n"
            + "dolu bir donem olacak. Sosyal cevrenizde dikkat cekeceginiz bir ay sizi bekliyor.\n\n"
            
            + "Kariyer: Ayin basinda Gunes’in Oglak burcundaki konumu, finansal konulara odaklanmanizi \n"
            + "sagliyor. Yeni gelir kaynaklari yaratabilir veya var olan birikimlerinizi degerlendirebilirsiniz. \n"
            + "19 Ocak’tan itibaren iletisim ve yaraticilik gerektiren islerinizde buyuk bir akicilik yasanacak.\n\n"
            
            + "Ask ve Iliskiler: Romantik ve eglenceli bir ay sizi bekliyor. Partnerinizle birlikte spontane \n"
            + "ve keyifli zamanlar gecirebilirsiniz. Eger bir iliskiniz yoksa, sosyal cevrenizden biriyle \n"
            + "tutkulu bir baslangic yapabilirsiniz. Ask hayatinizda surpriz gelismelere acik olun.\n\n"
            
            + "Saglik: Fiziksel aktiviteler ve acik hava sporlari enerjinizi artiracak. \n"
            + "Yogun tempodan dolayi duzenli beslenmeye dikkat etmeniz onemli.\n\n"
            
            + "Onemli Tarihler:\n"
            + "6 Ocak: Dolunay, finansal konularda onemli gelismeler getirebilir.\n" 
            + "20 Ocak: Yeni bir egitim veya seyahat plani yapabilirsiniz.",
             
         //Oğlak
             
             "Genel Bakis: Ocak ayi, Oglak burclari icin kisisel hedeflere odaklanacaklari \n"
            + "ve disiplinle ilerleyecekleri bir donem. Guclu enerjilerle kariyerinizde \n"
            + "onemli ilerlemeler kaydedebilirsiniz.\n\n"
            
            + "Kariyer: Gunes’in burcunuzdaki hareketi, liderlik becerilerinizi sergilemeniz \n"
            + "icin harika bir donem sunuyor. Ayin basinda sorumluluklariniz artsa da, disiplinli \n"
            + "calismaniz sayesinde buyuk basarilar elde edebilirsiniz. 19 Ocak’tan itibaren is \n"
            + "gorusmeleri ve projelerde daha hizli sonuclar alabilirsiniz.\n\n"
            
            + "Ask ve Iliskiler: İliskilerde ciddiyet ve istikrar aradiginiz bir donemdesiniz. \n"
            + "Partnerinizle gelecek planlari yapabilirsiniz. Yalnizsaniz, hayatiniza ciddi \n"
            + "bir iliski arayisinda olan biri girebilir.\n\n"
            
            + "Saglik: Enerjiniz yuksek olacak, ancak asiri calismaktan kacinin. \n"
            + "Dengeli bir yasam tarzi benimseyerek sagliginizi koruyabilirsiniz.\n\n"
            
            + "Onemli Tarihler:\n"
            + "6 Ocak: Dolunay, iliskilerde netlesme saglayabilir.\n" 
            + "31 Ocak: Yeni Ay, kisisel hedeflerinizde yeni bir baslangic sunuyor.",
             
         //Kova
             
             "Genel Bakis: Ocak, Kova burclari icin hem icsel bir farkindalik \n"
            + "hem de sosyal hareketlilik donemi olacak. Gelecege yonelik \n"
            + "hedeflerinizi sekillendirmek icin ideal bir zaman.\n\n"
            
            + "Kariyer: Ayin basinda kariyerinizle ilgili planlarinizi gozden \n"
            + "gecirerek stratejik adimlar atabilirsiniz. 19 Ocak’tan itibaren \n"
            + "is hayatinizda yenilikler ve iletisim trafigi hiz kazanacak. \n"
            + "Yaraticiliginizi sergileyerek dikkat cekebilirsiniz.\n\n"
            
            + "Ask ve Iliskiler: Ocak ayinin ilk yarisinda daha ice donuk bir \n"
            + "ruh hali icinde olabilirsiniz. Ay sonuna dogru, sosyal cevreniz \n"
            + "hareketlenecek ve yeni insanlarla tanisma fırsatiniz artacak. \n"
            + "Partnerinizle birlikte gelecege yonelik planlar yapabilirsiniz.\n\n"
            
            + "Saglik: Zihinsel yorgunlugu azaltmak icin kendinize zaman ayirmaniz \n"
            + "onemli. Meditasyon ve doga yuruyusleri ruhsal sagliginizi destekleyebilir.\n\n"
            
            + "Onemli Tarihler:\n"
            + "6 Ocak: Dolunay, gecmis meselelerde netlesme saglayabilir.\n" 
            + "20 Ocak: Gunes’in burcunuza gecmesiyle enerjiniz yukseliyor.",
             
         //Balık
             
             "Genel Bakis: Balik burclari icin Ocak ayi hayallerinizi gercege \n"
            + "donusturmek icin adim atabileceginiz bir donem olacak. Hem kariyer \n"
            + "hem de sosyal cevrede dikkat cekeceginiz bir ay sizi bekliyor.\n\n"
            
            + "Kariyer: Gunes’in Oğlak burcundaki konumu, is hayatinizda guclu baglantilar \n"
            + "kurmanizi ve projelerinizde ilerleme kaydetmenizi destekliyor. Ozellikle \n"
            + "ekip calismalari ve yaratici projelerde basarili olabilirsiniz. 19 Ocak’tan \n"
            + "itibaren iletisimde daha akici bir donem basliyor.\n\n"
            
            + "Ask ve Iliskiler: Partnerinizle romantik bir bag kurabilirsiniz. \n"
            + "Yalnizsaniz, ay sonunda hayatiniza yeni bir ask girebilir. Sosyal \n"
            + "cevrenizden biriyle baslayacak bir iliski surpriz olabilir.\n\n"
            
            + "Saglik: Fiziksel ve ruhsal dengenize ozen gostermelisiniz. \n"
            + "Meditasyon ve spor, enerjinizi yukseltecek. Dinlenmeyi ihmal etmeyin.\n\n"
            
            + "Onemli Tarihler:\n"
            + "6 Ocak: Dolunay, arkadaslik iliskilerinizde yeni bir farkindalik getirebilir.\n" 
            + "31 Ocak: Yeni Ay, kariyer hedeflerinizde yeni bir baslangic yapma firsati sunuyor."
            
    };    
}


public class YillikBurc extends Burc{
    
    public YillikBurc(String name) {
        super(name);
    }
    
    @Override
    public String[] getAnlamlar() {
        return yillikAnlamlar;
    }
    
    protected static String[] yillikAnlamlar={
        
        //Koç
        
            "Genel Bakis: 2025 yili, Koç burclari icin buyuk degisimlerin ve cesur \n"
            + "kararlarin yili olacak. Bu yil, Uranus’un etkisiyle beklenmedik degisimlere \n"
            + "acik olacaksiniz. Hem kariyerinizde hem de ozel hayatinizda yeni firsatlar \n"
            + "sizi bekliyor. Saturn’un etkisiyle, sorumluluklariniz artacak ve gelecege \n"
            + "yonelik daha saglam adimlar atmak icin gereksiz risklerden kacinmaniz gerekebilir.\n\n"
            
            + "Kariyer: Is hayatinizda cesur adimlar atarak kendinizi gosterebilir ve onemli \n"
            + "projelerde liderlik rolu ustlenebilirsiniz. Ancak dikkatli olmali, firsatlari \n"
            + "degerlendirmek icin fazla aceleci davranmamalisiniz. 2025, is degisikligi veya yeni bir \n"
            + "alanda kendinizi gelistirme firsati sunabilir. Parasal acidan buyuk kazanclar mumkun.\n\n"
            
            + "Ask ve Iliskiler: 2025, ask hayatinizda degisim ve yenilik yili olacak. Mevcut iliskinizde \n"
            + "bir sonraki adima gecmek, evlilik veya birlikte yeni bir yolculuga cikmak icin olumlu bir \n"
            + "yıl olabilir. Yalniz Koclar icin, daha ozgur ve cesur bir sekilde aski kesfetme firsatlari \n"
            + "dogacak. Uranus’un etkisiyle aniden bir iliskiye adim atabilirsiniz. Ancak, duygusal \n"
            + "anlamda daha stabil bir iliski isteginiz artabilir.\n\n"
            
            + "Saglik: 2025 yılı, enerjinizi yuksek tutmanin ve fiziksel sagliginiza daha fazla odaklanmanin \n"
            + "onemi konusunda uyarici olacak. Duzenli spor yaparak formda kalabilir, saglikli yasam \n"
            + "aliskanliklari benimseyebilirsiniz. Ayrica ruhsal sagliginiz da bu yil onemli olacak, \n"
            + "stresle basa cikmak icin meditasyon gibi rahatlatici aktiviteler faydali olabilir.",
        
        //Boğa
        
            "Genel Bakis: 2025 yili, Boga burclari icin finansal anlamda onemli bir yil olacak. \n"
            + "Uranus'un burcunuzdaki etkisi, sizi yeni baslangiclara ve surpriz degisimlere acik \n"
            + "tutacak. Kisisel gelisiminiz icin onemli firsatlar dogabilir ve 2025’te daha ozgur ve \n"
            + "bagimsiz bir sekilde hareket etme isteginiz artabilir. Hem is hayatinizda hem de ozel \n"
            + "hayatinizda daha fazla sorumluluk almaniz gerekebilir.\n\n"
            
            + "Kariyer: Kariyerinizde onemli bir donum noktasina gelebilir ve guclu finansal kararlar \n"
            + "alabilirsiniz. Bu yil, yeni bir is firsati ya da kariyerinizi ilerletecek bir egitim \n"
            + "programina katilma sansi dogabilir. Uranus sayesinde kariyerinizde surpriz gelismeler \n"
            + "yasanabilir ve is hayatinizda bazi yenilikci projelerde yer alabilirsiniz. Finansal anlamda \n"
            + "guvenli bir yil olacak ancak dikkatli ve stratejik adimlar atmaniz onemli.\n\n"
            
            + "Ask ve Iliskiler: Iliskilerinizde guven arayisiniz artacak ve partnerinizle birlikte \n"
            + "gelecege dair saglam adimlar atma ihtiyaci duyabilirsiniz. 2025, daha derin ve kalici \n"
            + "baglar kurma yili olabilir. Yalnizsaniz, stabil ve guven veren bir iliski isteginiz \n"
            + "daha fazla on planda olacak. Sosyal cevrenizden biriyle yeni bir iliskiye adim \n"
            + "atabilirsiniz. Ask hayatinda ani degisimler soz konusu olabilir.\n\n"
            
            + "Saglik: 2025 yilinda sagligiza ekstra dikkat etmeniz gerekecek. Duzenli egzersiz \n"
            + "yaparak fiziksel sagliginizi iyilestirebilir, psikolojik olarak da kendinizi \n"
            + "dengelemeye calismalisiniz. Uranus’un etkisiyle, aliskanliklarinizi \n"
            + "degistirebilir ve saglikli bir yasam tarzi benimseyebilirsiniz.",
        
        //İkizler
        
            "Genel Bakis: 2025, Ikizler burclari icin kisisel gelisim, yaratici projeler ve ailevi \n"
            + "konulara odaklanacaklari bir yil olacak. Uranus ve Pluto'nun etkisiyle, hayatinizda \n"
            + "koklu degisiklikler yapma isteginiz artacak. Kendinizi daha ozgur ve rahat hissetme \n"
            + "isteginiz baskin olacak. 2025 yilinda, kisisel hedefleriniz ve is hayatiniz \n"
            + "arasinda denge kurmaniz gerekebilir.\n\n"
            
            + "Kariyer: Kariyerinizde yenilikci ve yaratici projelere odaklanabilirsiniz. Ozellikle \n"
            + "2025'in ilk yarisinda isinizdeki bazi rutinlerden siyrilarak daha heyecan verici \n"
            + "projelere adim atma firsatlari olabilir. Uranus'un etkisiyle ani degisimler, isinizde \n"
            + "bir devrim yaratabilir. Ancak bu donemde daha fazla sorumluluk almaniz gerekebilir \n"
            + "ve bu sorumluluklar sizi hem zorlayabilir hem de buyutebilir.\n\n"
            
            + "Ask ve Iliskiler: Ask hayatinizda ani degisimler yasanabilir. Uranus'un etkisiyle \n"
            + "mevcut iliskinizde degisim ve donusum olasiligi artiyor. Eger yalnizsaniz, daha \n"
            + "ozgur ve maceraci bir ask arayisina girebilirsiniz. 2025 yilinda iliskinizde surpriz \n"
            + "gelismeler yasanabilir ve ciddi bir adim atmak mumkun olabilir. Yeni iliskiler, \n"
            + "2025'te daha cok basinizi dondurebilir.\n\n"
            
            + "Saglik: Saglik konusunda yil boyunca dikkatli olmaniz gereken bir donemdesiniz. \n"
            + "Stresle basa cikmak icin zihinsel sagliginiza ozen gostermeli, vucudunuzu dinlendirmeniz \n"
            + "gereken zamanlari iyi planlamalisiniz. Duzenli spor yapmak ve saglikli beslenmek \n"
            + "2025 yilinda size oldukca faydali olacak.",
        
        //Yengeç
        
            "Genel Bakis: 2025 yili Yengec burclari icin kariyer, aile ve icsel dengeye odaklanma \n"
            + "yili olacak. 2025 boyunca, gecmisten gelen sorumluluklar ve duygusal yuklerle basa \n"
            + "cikmaya calisabilirsiniz. Uranus ve Neptun'un etkisiyle, hayata dair onemli \n"
            + "farkindaliklar kazanarak kisisel donusum gecireceksiniz.\n\n"
            
            + "Kariyer: Yengec burclari, 2025 yilinda kariyerlerinde onemli bir ivme kazanacak. \n"
            + "Is hayatinizda atacaginiz adimlar, gelecekteki basarilariniz icin buyuk bir temel \n"
            + "olusturabilir. Ancak, kariyerinizdeki degisiklikler, sizi baslangicta zorlayabilir. \n"
            + "Yeni projeler, yeni is firsatlari veya kariyer degisikligi gundeme gelebilir. Is \n"
            + "arkadaslarinizla uyum icinde olmak ve onlari dinlemek isinizi kolaylastirabilir.\n\n"
            
            + "Ask ve Iliskiler: Ask hayatinizda, iliskilerde derinlesme ve bag kurma zamani. \n"
            + "Bu yil, partnerinizle daha fazla vakit gecirerek iliskinizde duygusal baglarinizi \n"
            + "guclendirebilirsiniz. Eger yalnizsaniz, size cok yakin bir cevreden biriyle iliskiye \n"
            + "baslayabilirsiniz. 2025 yilinda daha kalici ve saglikli iliskiler arayisinda olabilirsiniz.\n\n"
            
            + "Saglik: Yengec burclari icin 2025 yili, ruhsal dengeyi bulmak ve saglikli yasam \n"
            + "aliskanliklarini hayatiniza entegre etmek icin uygun bir donem. Stresle basa cikmak \n"
            + "icin meditasyon veya nefes egzersizleri yapabilirsiniz. Ayrica, fiziksel sagliginizi \n"
            + "ihmal etmemek ve egzersizlere agirlik vermek onemli olacak.",
        
        //Aslan
        
            "Genel Bakİs: 2025 yili, Aslan burclari icin kisisel gelisim, yaraticilik ve icsel \n"
            + "guclerini kesfetme yili olacak. Uranus ve Pluto'nun etkisiyle, eski \n"
            + "aliskanliklarinizdan ve guvenli bolgenizden cikmanız gerektigini hissedebilirsiniz. \n"
            + "Ancak, kendinizi bu surecte daha guclu ve ozgur hissedeceksiniz.\n\n"
            
            + "Kariyer: 2025, kariyerinizde yenilikci adimlar atma yili olabilir. Ozellikle \n"
            + "yaratici projelere yonelerek is hayatinizda yeni firsatlar yaratabilirsiniz. \n"
            + "Bu yil, ozellikle baslangicta kendinizi belirsiz bir ortamda bulabilirsiniz. \n"
            + "Ancak ilerleyen aylarda, tum cabalarinizin karsiligini alacak ve daha guclu bir \n"
            + "pozisyonda olacaksiniz. Uranus’un etkisiyle is hayatinizda surpriz degisiklikler \n"
            + "olabilir, ancak bunlar uzun vadede size fayda saglayacaktir.\n\n"
            
            + "Ask ve Iliskiler: Ask hayatinizda 2025, duygusal derinlik arayisina gireceginiz bir yil \n"
            + "olacak. Mevcut iliskinizde daha fazla guven ve samimiyet isteyebilirsiniz. Partnerinizle \n"
            + "aranizdaki bglari guclendirebilir, birlikte gelecege yonelik daha buyuk adimlar \n"
            + "atabilirsiniz. Yalnizsaniz, iliikinin baslangici sizin icin ozel ve farkli bir deneyim \n"
            + "olacak. Uranus, iliskinizde spontane ve heyecan verici bir degisim getirebilir.\n\n"
            
            + "Saglik: Saglik acisindan 2025, ruhsal sagliginiza ve stresle baca cikma yontemlerinize \n"
            + "odaklanacaginiz bir yıl olabilir. Fiziksel sagliginizda iyilesmeler yasayabilirsiniz ancak \n"
            + "uzun sureli stresten kacinmak icin rahatlatici aktivitelerle ilgilenmelisiniz. Duzenli \n"
            + "egzersiz yaparak fiziksel gucunuzu artirabilir, ruhsal dengeyi saglamak icin meditasyon ve \n"
            + "yoga gibi yontemleri deneyebilirsiniz.",
        
        //Başak
        
            "Genel Bakis: 2025 yili, Basak burclari icin aile, ev ve kisisel yasam konusunda buyuk bir \n"
            + "degisim yili olacak. Uranus ve Saturn'un etkisiyle, hayatinizdaki temelleri guclendirmek \n"
            + "ve geleceginizi planlamak icin firsatlar dogacak. Hem duygusal hem de maddi anlamda \n"
            + "daha guvenli bir yil gecirmek isteyeceksiniz.\n\n"
            
            + "Kariyer: Basak burclari, 2025 yilinda kariyerlerinde onemli bir ivme kazanabilirler. \n"
            + "Bu yil, kendinizi daha fazla liderlik pozisyonunda bulabilirsiniz. Ayrica, isinizde daha \n"
            + "fazla sorumluluk almak ve kariyerinizi bir ust seviyeye tasimak icin guclu firsatlar \n"
            + "dogacak. Uranus’un etkisiyle is yerinde bazi yenilikler, hatta degisimler yasanabilir, \n"
            + "ancak bu gelismeler sonunda uzun vadeli basarilar getirecek. Iyi bir planlama ve \n"
            + "strateji ile buyuk kazanimlar elde edebilirsiniz.\n\n"
            
            + "Ask ve Iliskiler: Ask hayatinizda, duygusal derinliklere inmeye ve daha saglam baglar \n"
            + "kurmaya meyilli olacaksiniz. Eger mevcut iliskinizde guven sorunlari varsa, bunlari \n"
            + "cozmek ve iliskinizi daha saglam temellere oturtmak icin bir donum noktasi olabilir. \n"
            + "Yalnizsaniz, bu yil daha ciddi ve uzun vadeli bir iliski kurma sansiniz yuksek. \n"
            + "Uranus’un etkisiyle, iliskilere dair surpriz gelismeler olabilir.\n\n"
            
            + "Saglik: 2025 yili, Basak burclari icin ruhsal ve fiziksel saglik acisindan onemli bir \n"
            + "yil olacak. Sagliginizla ilgilenmek ve kendinizi iyilestirmek icin gereken zamani \n"
            + "ayirmalisiniz. Duzenli spor yapmak ve saglikli bir yasam tarzini benimsemek, uzun \n"
            + "vadede daha saglikli olmaniza yardimci olacak. Ayrica, stresi azaltmak ve zihinsel \n"
            + "sagliginizi korumak icin rahatlatici ontemlere yonelmek onemli olacak.",
        
        //Terazi
        
            "Genel Bakis: 2025 yili, Terazi burclari icin kisisel gelisim, egitim ve sosyal cevreye \n"
            + "odaklanacak bir yil olacak. Uranus ve Pluto’nun etkisiyle, kendi fikirlerinizi ve \n"
            + "degerlerinizi yeniden gozden gecirebilirsiniz. Hayatinizdaki bazi kaliplari kirarak \n"
            + "yeni bir perspektif gelistireceksiniz.\n\n"
            
            + "Kariyer: Kariyer hayatinizda 2025 yilinda onemli firsatlar olabilir. Yeni projelere adim \n"
            + "atabilir, is hayatinizda kendinizi daha cok ifade etme sansi bulabilirsiniz. Ancak, yenilikci \n"
            + "dusunme ve risk alma konusunda temkinli olmalisiniz. Ozellikle is arkadaslarinizla uyumlu \n"
            + "calismak, hedeflerinize ulasmanizi hizlandiracaktir. Ayrica, Uranus’un etkisiyle egitim \n"
            + "ve ogretim alanlarinda yeni firsatlar dogabilir.\n\n"
            
            + "Ask ve Iliskiler: Ask hayatinizda 2025 yili, daha ozgur ve bagimsiz iliskiler arayisina \n"
            + "girebileceginiz bir donem olacak. Mevcut iliskinizde daha fazla ozgurluk isteyebilirsiniz. \n"
            + "Yalnizsaniz, sosyal cevrenizden biriyle tanisabilirsiniz. 2025, aski ve iliskileri daha \n"
            + "farkli bir sekilde deneyimleme yili olabilir. Uranus, ani ve heyecan verici bir \n"
            + "iliskiye adim atmaniza neden olabilir.\n\n"
            
            + "Saglik: 2025 yili saglik acisindan yeniliklere acik bir donem olacak. Vucudunuzun \n"
            + "ihtiyaclarina dikkat etmek, saglikli aliskanliklar edinmek on plana cikacak. Zihinsel \n"
            + "sagliginizla ilgilenmek de onemli olacak; meditasyon, yoga veya psikolojik destek \n"
            + "almak bu yil sizi rahatlatabilir.",
        
        //Akrep
        
            "Genel Bakis: 2025 yili, Akrep burclari icin is ve ozel hayatlarinda daha fazla derinlik \n"
            + "ve donusum arayisinda olacaklari bir yil olacak. Uranus’un etkisiyle finansal ve \n"
            + "duygusal alanlarda buyuk degisimlere acik olacaksiniz. Gecmiateki kaliplarinizi \n"
            + "kirarak daha ozgur bir yasam tarzi benimseyeceksiniz.\n\n"
            
            + "Kariyer: Akrep burclari, 2025 yilinda kariyerlerinde buyuk degisimlere adim atabilir. \n"
            + "Yenilikci projelere yonelmek ve liderlik pozisyonlarina gelmek icin guclu bir yil \n"
            + "olacak. Ancak, risk alirken dikkatli olmalisiniz, pzellikle finansal kararlar konusunda \n"
            + "temkinli olmaniz gerekebilir. Uranus’un etkisiyle is hayatinizda surpriz gelismeler \n"
            + "yasanabilir. Bu yil, cok istediginiz bir terfi ya da is degisikligi firsatlari dogabilir.\n\n"
            
            + "Ask ve Iliskiler: Ask hayatinizda 2025 yili, derinlesme ve donusum yili olacak. \n"
            + "Mevcut iliskinizde, daha derin bir bag kurmak ve duygusal olarak birbirinizi anlamak \n"
            + "isteyebilirsiniz. Eger yalnizsaniz, surpriz bir ask hayatiniza girebilir. Uranus, \n"
            + "iliskinizde ani gelismeler yasanmasina neden olabilir. Kendi ic dunyanizda da degisim \n"
            + "yasayarak daha ozgur bir ask anlayisina sahip olabilirsiniz.\n\n"
            
            + "Saglik: Saglik acisindan bu yil, fiziksel ve ruhsal dengeyi bulmaya calisacaginiz bir \n"
            + "donem olacak. Saglikli yasam tarzini benimsemek ve vucudunuzu dinlendirmek onem kazanacak. \n"
            + "Ayrica, zihinsel sagliginizi korumak icin stres yonetimi konusunda dikkatli olmalisiniz.",
        
        //Yay
        
            "Genel Bakis: 2025 yili, Yay burclari icin kisisel degerler, finansal istikrar ve icsel \n"
            + "kesif yili olacak. Uranus’un etkisiyle maddi kaynaklarinizi yeniden duzenleme \n"
            + "ve daha saglam temeller atma firsatlari dogabilir. Bu yil, hayatinizda yeniliklere, \n"
            + "degisimlere acik olacaginiz bir donem olacak, ancak bu degisimlerin size uzun \n"
            + "vadede guven ve huzur getirecegini fark edeceksiniz.\n\n"
            
            + "Kariyer: Yay burclari icin kariyer alaninda 2025 yili onemli firsatlar sunacak. \n"
            + "Ozellikle maddi kazanclarinizi arttiracak yeni projeler veya is firsatlari dogabilir. \n"
            + "Is hayatinizda yeni bir duzen olusturabilir, uzun vadede size fayda saglayacak \n"
            + "adimlar atabilirsiniz. Uranus sayesinde ani kariyer degigimleri ve surpriz basarilar \n"
            + "yasanabilir. Ancak, risk almak konusunda dikkatli olmaniz gerekebilir, zira \n"
            + "aceleci kararlar size zarar verebilir.\n\n"
            
            + "Ask ve Iliskiler: Ask hayatinizda 2025 yili, daha ciddi ve guven veren iliskilere \n"
            + "yonelme yili olabilir. Mevcut iliskinizde daha fazla guven arayisiniz olacak ve \n"
            + "bu da iliskinizin daha saglam temellere dayanmasini saglayacak. Eger yalnizsaniz, \n"
            + "size hitap eden, derin bir bag kurabileceginiz birisiyle tanisabilirsiniz. \n"
            + "Ask hayatinizda Uranus’un etkisiyle surpriz gelismeler yasanabilir, fakat \n"
            + "bu gelismeler baslangicta size karmasik gelebilir.\n\n"
            
            + "Saglik: 2025 yili saglik acisindan sizi zinde tutacak ve yasam enerjinizi artiracak \n"
            + "bir yil olacak. Duzenli spor ve saglikli beslenme aliskanliklari, enerjinizi yuksek \n"
            + "tutmaniza yardimci olacak. Ayrica, ruhsal sagliginiza da dikkat etmeniz gereken bir yil. \n"
            + "Stresle basa cikabilmek icin rahatlatici aktivitelerle ilgilenmelisiniz. \n"
            + "Zihinsel dengeyi bulmak icin meditasyon veya yoga gibi yontemleri deneyebilirsiniz.",
        
        //Oğlak
        
            "Genel Bakis: 2025 yili, Oglak burclari icin toplumsal statu, iliskiler ve kisisel hedeflere \n"
            + "odaklanma yili olacak. Uranus ve Pluto’nun etkisiyle, daha fazla ozgurluk ve yenilik \n"
            + "arayisiniz artacak. 2025 yili, hem ozel hayatinizda hem de is hayatinizda buyuk \n"
            + "donusumlere acik olacaginiz bir donem olacak. Bu yil, duygusal ve finansal \n"
            + "anlamda buyuk ilerlemeler kaydedebilirsiniz.\n\n"
            
            + "Kariyer: 2025 yili, kariyerinizde onemli bir donum noktasi olabilir. Yuksek hedefler \n"
            + "pesinde kosacak ve kariyerinizi bir ust seviyeye tasima firsatlari yakalayacaksiniz. \n"
            + "Uranus sayesinde, is hayatinizda surpriz degisiklikler olabilir. Bu yil, isinizde daha \n"
            + "fazla yenilik ve farklilik arayisi içinde olabilirsiniz. Eger is degisikligi yapmak \n"
            + "istiyorsaniz, 2025 yili bu adimi atmak icin uygun bir zaman olabilir. Ancak, yeni \n"
            + "firsatlar konusunda aceleci olmamalisiniz, iyi bir planlama yapmaniz gerekecek.\n\n"
            
            + "Ask ve Iliskiler: Ask hayatinizda 2025, daha derin ve anlamli iliskiler kurma yili olabilir. \n"
            + "Mevcut iliskinizde duygusal baglarinizi daha guclu bir hale getirebilir, gelecege dair \n"
            + "daha ciddi adimlar atabilirsiniz. Yalnizsaniz, guvene dayali bir iliski arayisinda olacak \n"
            + "ve bu yil, size hitap eden bir partnerle tanisabilirsiniz. Uranus’un etkisiyle, \n"
            + "iliskilerde ani ve beklenmedik gelismeler yasanabilir.\n\n"
            
            + "Saglik: 2025 yilinda sagliginiz icin guclu bir yil olacak. Ancak, dikkatli olmaniz \n"
            + "gereken nokta, is ve ozel yasam dengesini iyi kurmak olacak. Stresli durumlar sagliginizi \n"
            + "etkileyebilir, bu nedenle stres yonetimi konusunda ozen gostermelisiniz. Fiziksel sagliginizi \n"
            + "korumak icin duzenli egzersiz yapmaniz onemli. Ayrica, ruhsal sagliginizi dengelemek \n"
            + "icin kendinize zaman ayirmali ve rahatlatici aktivitelerle stres atmalisiniz.",
        
        //Kova
        
            "Genel Bakis: 2025 yili, Kova burclari icin kariyer, toplumsal statu ve kisisel hedeflere ulasmak \n"
            + "icin onemli firsatlar sunacak. Uranus ve Pluto’nun etkisiyle, is hayatinizda radikal \n"
            + "degisiklikler yapabilir ve toplumsal alanda daha fazla gorunur olabilirsiniz. Bu yil, \n"
            + "yasaminiza yeni bir yon verme ve kisisel bagimsizliginizi guclendirme yili olacak.\n\n"
            
            + "Kariyer: 2025, kariyerinizde onemli degisimlerin yasanacagi bir yil olacak. Uranus’un \n"
            + "etkisiyle, is hayatinizda ani degisiklikler ve surpriz firsatlar olabilir. Bu yil, \n"
            + "kendinizi yeni projelere ve yeni is alanlarina yonlendirebilirsiniz. Ayrica, kariyerinizde \n"
            + "ilerlemek ve toplumsal statunuzu artirmak icin yeni stratejiler gelistireceksiniz. \n"
            + "Yaratici ve yenilikci projelere katilabilir, kariyerinizde kendinizi daha guclu \n"
            + "bir sekilde ifade edebilirsiniz.\n\n"
            
            + "Ask ve Iliskiler: Ask hayatinizda 2025 yili, daha ozgur ve bagimsiz bir donem olabilir. \n"
            + "Mevcut iliskinizde, partnerinizle kisisel ozgurluklerinizi daha iyi anlamaya calisabilir \n"
            + "ve birbirinize alan taniyarak daha guclu bir bag kurabilirsiniz. Eger yalnizsaniz, bu yil, \n"
            + "kendinizi daha ozgur hissedeceginiz bir iliskiye adim atabilirsiniz. Uranus’un etkisiyle, \n"
            + "ask hayatinizda surpriz gelismeler yasanabilir.\n\n"
            
            + "Saglik: 2025 yilinda sagliginiza dikkat etmeniz gereken bir yil olacak. Fiziksel \n"
            + "sagliginizla ilgilenmek ve duzenli egzersiz yaparak enerji seviyenizi yuksek tutmak \n"
            + "onemli olacak. Ayrica, stresle basa cikmak icin rahatlatici aktivitelerle ilgilenmek, \n"
            + "zihinsel sagliginizi korumak icin faydali olacak.",
        
        //Balık
        
            "Genel Bakis: 2025 yili, Balik burclari icin finansal guvenlik, kisisel hedefler ve \n"
            + "kariyer gelisimi acisindan onemli bir yil olacak. Uranus ve Neptun’un etkisiyle, \n"
            + "hayatta daha fazla denge ve icsel huzur arayisina girebilirsiniz. Bu yil, maddi \n"
            + "acidan saglam temeller atmak icin uygun firsatlar dogacak.\n\n"
            
            + "Kariyer: 2025 yili, kariyerinizde buyuk ilerlemeler kaydedebileceginiz bir yil olacak. \n"
            + "Uranus sayesinde, is hayatinizda yenilikci adimlar atabilir ve yaratici projelere yonelerek \n"
            + "fark yaratabilirsiniz. Finansal anlamda guvenli bir yil olacak ve uzun vadeli projelere \n"
            + "yonelebilirsiniz. Isinizde daha fazla sorumluluk alarak kariyerinize yeni bir yon \n"
            + "verebilirsiniz. Bu yil, kariyerinizi bir ust seviyeye tasiyacak firsatlar dogabilir.\n\n"
            
            + "Ask ve Iliskiler: Ask hayatinizda 2025, daha derin ve guvene dayali iliskiler kurma yili \n"
            + "olacak. Mevcut iliskinizde daha fazla sadakat ve guven arayisiniz olacak. Yalnizsaniz, \n"
            + "bu yil, sizinle ayni degerleri paylasan biriyle tanisabilirsiniz. Uranus’un etkisiyle, \n"
            + "ask hayatinizda surpriz gelismeler yasanabilir. Iliskilerdeki degisimlere acik olmali \n"
            + "ve yeni firsatlar karsisinda cesur adimlar atmalisiniz.\n\n"
            
            + "Saglik: 2025 yili, Balik burclari icin saglik acisindan dengeyi bulma yili olacak. \n"
            + "Vucudunuzu dinlendirmeniz ve saglikli aliskanliklar edinmeniz onemli olacak. \n"
            + "Ayrica, ruhsal sagliginizda da dengeyi bulmak icin meditasyon ve rahatlatici \n"
            + "aktiviteler yaparak icsel huzuru koruyabilirsiniz."
    };
}



import java.util.Scanner;

public class BurcYorumu {
    
    public int gun;
    public int ay;
    public String secim;
    public String burc;
    public int tercih;
    
    
    Scanner klavye = new Scanner(System.in);
    
    
    public BurcYorumu(){
        
        System.out.println("Burcunuzu biliyor musunuz?");
        //System.out.println("Biliyorsaniz 1, bilmiyorsaniz 2 rakamini tuslayiniz.");
        secim=klavye.next().toLowerCase();
    }
    
    
    public String burcHesabi(){
       
        switch (secim) {
            case "evet":
                System.out.print("Lutfen burcunuzu giriniz: ");
                burc=klavye.next().toUpperCase();
                System.out.println();
                break;
            case "hayır":
                System.out.print("Dogum ayinizi giriniz(1-12): ");
                ay=klavye.nextInt();
                System.out.print("Dogum gununuzu seciniz (1-31):");
                gun=klavye.nextInt();
                if ((ay == 1 && gun >= 21) || (ay == 2 && gun <= 19)) {
                    burc = "Kova".toUpperCase();
                }
                
                else if ((ay == 2 && gun >= 20) || (ay == 3 && gun <= 20)) {
                    burc = "Balık".toUpperCase();
                }
                
                else if ((ay == 3 && gun >= 21) || (ay == 4 && gun <= 20)) {
                    burc = "Koc".toUpperCase();
                }
                
                else if ((ay == 4 && gun >= 21) || (ay == 5 && gun <= 21)) {
                    burc = "Boga".toUpperCase();
                }
                
                else if ((ay == 5 && gun >= 22) || (ay == 6 && gun <= 22)) {
                    burc = "Ikızler".toUpperCase();
                }
                
                else if ((ay == 6 && gun >= 23) || (ay == 7 && gun <= 22)) {
                    burc = "Yengec".toUpperCase();
                }
                
                else if ((ay == 7 && gun >= 23) || (ay == 8 && gun <= 22)) {
                    burc = "Aslan".toUpperCase();
                }
                
                else if ((ay == 8 && gun >= 23) || (ay == 9 && gun <= 22)) {
                    burc = "Basak".toUpperCase();
                }
                
                else if ((ay == 9 && gun >= 23) || (ay == 10 && gun <= 22)) {
                    burc = "Terazı".toUpperCase();
                }
                else if ((ay == 10 && gun >= 23) || (ay == 11 && gun <= 21)) {
                    burc = "Akrep".toUpperCase();
                }
                
                else if ((ay == 11 && gun >= 22) || (ay == 12 && gun <= 21)) {
                    burc = "Yay".toUpperCase();
                }
                
                else if ((ay == 12 && gun >= 22) || (ay == 1 && gun <= 20)) {
                    burc = "Oglak".toUpperCase();
                }
                
                else {
                    burc = "Gecersiz bir tarih girdiniz.";
                }   
                break;
            default:
                System.out.println("Gecersiz bir tercih yaptiniz!");
                break;
               
        }
        
       
        System.out.println("Burcunuz: "+burc);
        return burc;
    }
    
    public void burcYorumu(){
        
        
        YillikBurc yillik = new YillikBurc(burc);
        AylikBurc aylik = new AylikBurc(burc);
        
        System.out.println("Simdi de istediginiz burc yorumunu seciniz: ");
        System.out.println("1 - Aylik Yorum");
        System.out.println("2 - Yillik Yorum");
        System.out.print("Seciminiz: ");
        tercih=klavye.nextInt();
        
        System.out.println();
        
        if(burc.equals("koc".toUpperCase()) && tercih==1){
            
            System.out.println(aylik.getAnlamlar()[0]);
        }
        
        else if(burc.equals("koc".toUpperCase()) && tercih==2){
            System.out.println(yillik.getAnlamlar()[0]);
        }
        
        else if(burc.equals("boga".toUpperCase()) && tercih==1){
            System.out.println(aylik.getAnlamlar()[1]);
        }
        
        else if(burc.equals("boga".toUpperCase()) && tercih==2){
            System.out.println(yillik.getAnlamlar()[1]);
        }
        
        else if(burc.equals("ıkızler".toUpperCase()) && tercih==1){
            System.out.println(aylik.getAnlamlar()[2]);
        }
        
        else if(burc.equals("ıkızler".toUpperCase()) && tercih==2){
            System.out.println(yillik.getAnlamlar()[2]);
        }
        
        else if(burc.equals("yengec".toUpperCase()) && tercih==1){
            System.out.println(aylik.getAnlamlar()[3]);
        }
        
        else if(burc.equals("yengec".toUpperCase()) && tercih==2){
            System.out.println(yillik.getAnlamlar()[3]);
        }
        
        else if(burc.equals("aslan".toUpperCase()) && tercih==1){
            System.out.println(aylik.getAnlamlar()[4]);
        }
        
        else if(burc.equals("aslan".toUpperCase()) && tercih==2){
            System.out.println(yillik.getAnlamlar()[4]);
        }
        
        else if(burc.equals("basak".toUpperCase()) && tercih==1){
            System.out.println(aylik.getAnlamlar()[5]);
        }
        
        else if(burc.equals("basak".toUpperCase()) && tercih==2){
            System.out.println(yillik.getAnlamlar()[5]);
        }
        
        else if(burc.equals("terazı".toUpperCase()) && tercih==1){
            System.out.println(aylik.getAnlamlar()[6]);
        }
        
        else if(burc.equals("terazı".toUpperCase()) && tercih==2){
            System.out.println(yillik.getAnlamlar()[6]);
        }
        
        else if(burc.equals("akrep".toUpperCase()) && tercih==1){
            System.out.println(aylik.getAnlamlar()[7]);
        }
        
        else if(burc.equals("akrep".toUpperCase()) && tercih==2){
            System.out.println(yillik.getAnlamlar()[7]);
        }
        
        else if(burc.equals("yay".toUpperCase()) && tercih==1){
            System.out.println(aylik.getAnlamlar()[8]);
        }
        
        else if(burc.equals("yay".toUpperCase()) && tercih==2){
            System.out.println(yillik.getAnlamlar()[8]);
        }
        
        else if(burc.equals("oglak".toUpperCase()) && tercih==1){
            System.out.println(aylik.getAnlamlar()[9]);
        }
        
        else if(burc.equals("oglak".toUpperCase()) && tercih==2){
            System.out.println(yillik.getAnlamlar()[9]);
        }
        
        else if(burc.equals("kova".toUpperCase()) && tercih==1){
            System.out.println(aylik.getAnlamlar()[10]);
        }
        
        else if(burc.equals("kova".toUpperCase()) && tercih==2){
            System.out.println(yillik.getAnlamlar()[10]);
        }
        
        else if(burc.equals("balık".toUpperCase()) && tercih==1){
            System.out.println(aylik.getAnlamlar()[11]);
        }
        
        else if(burc.equals("balık".toUpperCase()) && tercih==2){
            System.out.println(yillik.getAnlamlar()[11]);
        }
        
    }
}



import java.util.Scanner;

public class BurcIslemleri {
    
    public int gun;
    public int ay;
    public String secim1;
    public String secim2;
    public String burc;
    public int burcSayisi;
    public int tercih;
    public int secilenAy;
    
    AylikBurc aylik = new AylikBurc();
    YillikBurc yillik = new YillikBurc();
    
    Scanner klavye= new Scanner(System.in);
    
    public String[] ozellikler={
        
        //Koç
        
        "Bu burcun mensupları, genellikle enerjik, cesur ve kararlı yapılarıyla tanınır. \n"
            + "Koç burcunun özellikleri arasında hızlı hareket etme ve ani kararlar alma \n"
            + "yetenekleri de bulunur. Koç burçları, genellikle bağımsızlığına düşkün ve \n"
            + "kendi yolunu çizmeyi seven bireylerdir.",
        
        //Boğa
        
        "Boğa burcu insanı cana yakın, merhametli ve sempatik yapısıyla biliniyor. \n"
            + "Toprak grubunda yer alan Boğa burçları, sakin ve güvenilir yapılarıyla da \n"
            + "tanınıyor. Keskin düzeyde maddi zekaya sahip olan bu insanlar hem gündelik \n"
            + "yaşamda hem de iş hayatında bu özellikleri ile kolaylık sağlıyorlar.",
        
        //İkizler
        
        "İkizler burcu, enerjik ve çok yönlü yapısıyla öne çıkar. Bir ortama girdiğinde \n"
            + "sürekli gülümsemesi, mutlu tavırları ve canayakınlığıyla göze çarpan bu \n"
            + "kişiler, hareketli yaşamayı sever. Ancak ikizler burcu özellikleri arasında \n"
            + "yer alan kararsızlık ve değişkenlik, zaman zaman maymun iştahlılığa dönüşebilir.",
        
        //Yengeç
        
        "Yengeç'ler duygusallıkları ve duyarlılıkları ile tanınırlar. Çevresindeki her insandan \n"
            + "da aynı hassasiyeti bekledikleri için, kolay geçinilebilir kişiler değildir. \n"
            + "İyi günlerinde neşeli, iyi kalpli, yardımsever, düşünceli ve anlayışlıdırlar. \n"
            + "Fakat herhangi belirgin bir neden olmadan somurtkan ve alıngan olabilirler.",
        
        //Aslan
        
        "Aslan Burcu, Zodyak'ın beşinci burcu olarak tanınır ve 23 Temmuz ile 22 Ağustos tarihleri \n"
            + "arasında doğanları temsil eder. Bu burcun insanları, kendilerine güvenen, cesur ve \n"
            + "doğal liderler olarak bilinirler. Ateş elementiyle ilişkilendirilen Aslan bireyleri, \n"
            + "adeta içlerinde yanan bir alev gibi enerjik ve tutkuludurlar.",
        
        //Başak
        
        "Başak burcu, detaycılığı ve analitik düşünce yapısıyla tanınır. Başak burcu \n"
            + "insanları, mantıklı ve pratik yaklaşımıyla sorunlara çözüm üretmede ustadır. \n"
            + "Başak burcunun özellikleri arasında dikkatli ve özenli olma, \n"
            + "küçük detaylara bile büyük önem verme bulunur.",
        
        //Terazi
        
        "Terazi burçları genel olarak akıllı, mantıklı ve aşk dolu özelliklere sahiplerdir. \n"
            + "Terazi burçları hayallerine ulaşmak için çok çalışırlar. Terazi burçları genel \n"
            + "olarak uzlaşı yanlısı ve kibar özellikleri ile bilinirler. İlişkilerinde \n"
            + "adil olan terazi burçları mantıkları ile birlikte hareket ederler.",
        
        //Akrep
        
        "Sabit bir su burcu olan Akrepler sadakatleri, bağlılıkları ve tutkularıyla tanınırlar. \n"
            + "İçgüdüleri ve doğuştan gelen durugörü yetenekleri ile insanların kendilerinin \n"
            + "bile farkında olmadığı yönlerini görme yeteneğine sahiptirler. Bu onların \n"
            + "hem en güçlü yönü hem de lanetidir.",
        
        //Yay
        
        " Yay burcunun temel nitelikleri arasında maceraperestlik, yenilik arayışı ve \n"
            + "iyimserlik öne çıkar. Yay burcu kadınları ve erkekleri, özgürlüğüne \n"
            + "düşkün ve maceracı ruhlarıyla tanınırlar.",
        
        //Oğlak
        
        "Temel özellikleri arasında kararlılık, disiplin, ciddiyet ve hedefe yönelik bir \n"
            + "bakış açısı bulunur. Oğlak burcu bireyleri genellikle çalışkan, \n"
            + "sorumluluk sahibi ve liderlik özellikleriyle bilinir.",
        
        //Kova
        
        "Hava grubuna ait olan Kova burcu, yenilikçi, özgür ruhlu ve bağımsız karakteriyle bilinir. \n"
            + "Bu burçta doğan insanlar, genellikle toplumsal meselelerle ilgilenir ve insan haklarına \n"
            + "büyük önem verirler. Kova burcu özellikleri arasından en belirginlerinden biri, \n"
            + "sıradışı düşünce yapılarına sahip olmalarıdır.",
        
        //Balık
        
        "Genel olarak uysallığı ile bilinen ve su grubu olan balık burçları 20 Şubat ile \n"
            + "20 Mart tarihleri arasında doğmuş kişilerdir. Balık burcu olan kişiler \n"
            + "genel olarak sabırlı, eli açık ve de duyarlı olan insanlardır. \n"
            + "Bu kişilerin her daim büyük bir inandırma yetenekleri bulunmaktadır."  
    };
    
    public BurcIslemleri(){
        
        
    }
    
    
    public String burcHesabi(){
        
        System.out.println("Burcunuzu biliyor musunuz?");
        secim1=klavye.next().toLowerCase();
       
        switch (secim1) {
            case "evet":
                System.out.print("Lutfen burcunuzu giriniz: ");
                burc=klavye.next().toUpperCase();
                System.out.println();
                
                switch(burc){
                    
                    case "KOVA":
                        burcSayisi=10;
                        break;
                        
                    case "BALIK":
                        burcSayisi=11;
                        break;
                        
                    case "KOC":
                        burcSayisi=0;
                        break;
                        
                    case "BOGA":
                        burcSayisi=1;
                        break;
                        
                    case "IKIZLER":
                        burcSayisi=2;
                        break;
                        
                    case "YENGEC":
                        burcSayisi=3;
                        break;
                        
                    case "ASLAN":
                        burcSayisi=4;
                        break;
                        
                    case "BASAK":
                        burcSayisi=5;
                        break;
                        
                    case "TERAZI":
                        burcSayisi=6;
                        break;
                        
                    case "AKREP":
                        burcSayisi=7;
                        break;
                        
                    case "YAY":
                        burcSayisi=8;
                        break;
                        
                    case "OGLAK":
                        burcSayisi=9;
                        break;
                }
                
                break;
                
            case "hayır":
                System.out.print("Dogum ayinizi giriniz(1-12): ");
                ay=klavye.nextInt();
                System.out.print("Dogum gununuzu seciniz (1-31):");
                gun=klavye.nextInt();
                if ((ay == 1 && gun >= 21) || (ay == 2 && gun <= 19)) {
                    burc = "Kova".toUpperCase();
                    burcSayisi=10;
                }
                
                else if ((ay == 2 && gun >= 20) || (ay == 3 && gun <= 20)) {
                    burc = "Balık".toUpperCase();
                    burcSayisi=11;
                }
                
                else if ((ay == 3 && gun >= 21) || (ay == 4 && gun <= 20)) {
                    burc = "Koc".toUpperCase();
                    burcSayisi=0;
                }
                
                else if ((ay == 4 && gun >= 21) || (ay == 5 && gun <= 21)) {
                    burc = "Boga".toUpperCase();
                    burcSayisi=1;
                }
                
                else if ((ay == 5 && gun >= 22) || (ay == 6 && gun <= 22)) {
                    burc = "Ikızler".toUpperCase();
                    burcSayisi=2;
                }
                
                else if ((ay == 6 && gun >= 23) || (ay == 7 && gun <= 22)) {
                    burc = "Yengec".toUpperCase();
                    burcSayisi=3;
                }
                
                else if ((ay == 7 && gun >= 23) || (ay == 8 && gun <= 22)) {
                    burc = "Aslan".toUpperCase();
                    burcSayisi=4;
                }
                
                else if ((ay == 8 && gun >= 23) || (ay == 9 && gun <= 22)) {
                    burc = "Basak".toUpperCase();
                    burcSayisi=5;
                }
                
                else if ((ay == 9 && gun >= 23) || (ay == 10 && gun <= 22)) {
                    burc = "Terazı".toUpperCase();
                    burcSayisi=6;
                }
                else if ((ay == 10 && gun >= 23) || (ay == 11 && gun <= 21)) {
                    burc = "Akrep".toUpperCase();
                    burcSayisi=7;
                }
                
                else if ((ay == 11 && gun >= 22) || (ay == 12 && gun <= 21)) {
                    burc = "Yay".toUpperCase();
                    burcSayisi=8;
                }
                
                else if ((ay == 12 && gun >= 22) || (ay == 1 && gun <= 20)) {
                    burc = "Oglak".toUpperCase();
                    burcSayisi=9;
                }
                
                else {
                    System.out.println("Gecersiz bir tarih girdiniz.");
                }   
                break;
            default:
                System.out.println("Gecersiz bir tercih yaptiniz!");
                break;
        }
        System.out.println("Burcunuz: "+burc);
        return burc;
    }
    
    public void burcOzelligi(){
        
        System.out.println("Burcunuzun ozelligini ogrenmek ister misiniz?");
        secim2=klavye.next().toLowerCase();
        
        switch(secim2){
            
            case "evet":
               
                if(burc.equals("Koc".toUpperCase())){
                    System.out.println("Koc Burcunun Ozelligi: "+ozellikler[0]);
                }
                
                else if(burc.equals("Boga".toUpperCase())){
                    System.out.println("Boga Burcunun Ozelligi: "+ozellikler[1]);
                }
                
                else if(burc.equals("Ikızler".toUpperCase())){
                    System.out.println("ıkizler Burcunun Ozelligi: "+ozellikler[2]);
                }
                
                else if(burc.equals("Yengec".toUpperCase())){
                    System.out.println("Yengec Burcunun Ozelligi: "+ozellikler[3]);
                }
                
                else if(burc.equals("Aslan".toUpperCase())){
                    System.out.println("Aslan Burcunun Ozelligi: "+ozellikler[4]);
                }
                
                else if(burc.equals("Basak".toUpperCase())){
                    System.out.println("Basak Burcunun Ozelligi: "+ozellikler[5]);
                }
                
                else if(burc.equals("Terazı".toUpperCase())){
                    System.out.println("Terazi Burcunun Ozelligi: "+ozellikler[6]);
                }
                
                else if(burc.equals("Akrep".toUpperCase())){
                    System.out.println("Akrep Burcunun Ozelligi: "+ozellikler[7]);
                }
                
                else if(burc.equals("Yay".toUpperCase())){
                    System.out.println("Yay Burcunun Ozelligi: "+ozellikler[8]);
                }
                
                else if(burc.equals("Oglak".toUpperCase())){
                    System.out.println("Oglak Burcunun Ozelligi: "+ozellikler[9]);
                }
                
                else if(burc.equals("Kova".toUpperCase())){
                    System.out.println("Kova Burcunun Ozelligi: "+ozellikler[10]);
                }
                
                else if(burc.equals("Balık".toUpperCase())){
                    System.out.println("Balik Burcunun Ozelligi: "+ozellikler[11]);
                }
                break;
            
                
            case "hayir":
                
                System.out.println("Nasil istersen.");
                break;
        }
    }
    
    public void burcYorumu(){
        
        System.out.println("Iki tur burc yorumu mevcuttur.");
        System.out.println("1)Aylik Burc Yorumu");
        System.out.println("2)Yillik Burc Yorumu");
        System.out.println("Istediginiz yorum turu hangisi?");
        tercih=klavye.nextInt();
        
        switch(tercih){
            
            case 1:
                
                System.out.println("Kacinci ayin yorumunu istersin?");
                secilenAy=klavye.nextInt();
                
                System.out.println(secilenAy+". Ayin Yorumu " +aylik.getAnlamlar()[secilenAy-1][burcSayisi]);
                break;
                
            case 2:
                
                System.out.println(burc+" Burcunun Yillik Yorumu: ");
                System.out.println(""+yillik.getAnlamlar()[burcSayisi]);
                break;
                
            default:
                
                System.out.println("Gecersiz bir tercih yaptiniz!");
                break;
        }
    }
}

