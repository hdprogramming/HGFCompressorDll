# HGFCompressorDll
.HGF Encoder/Decoder Dynamic Library File
C# vs. projelerde kullanım için HGFDönüştürücü artık .dll şeklinde;

CompressPicture(System.Drawing.Bitmap, [string], [int], [HGFCompressor.HGFComp.EncoderMode], [byte], [bool])
metoduyla bitmap resminizi .hgf dönüştürebilirsiniz.
Örnek Kullanımı
HGFComp hgfc=new HGFComp();
hgfc.CompressPicture(Bitmap DonusturelecekResim,String DosyaAdı,int kalite,EncoderMode encodermodu,byte preencode,bool gray);
Direkt
hgfc.CompressPicture(Bitmap DonusturelecekResim,String DosyaAdı) şeklinde yazabileceğiniz gibi;
Parametreler girip daha profesyonelcede kullanabilirsiniz;
Parametreler:
kalite:Kalite ayarı
encodermodu:
EncoderMode.DWT32x32=32x32 bloklar şeklinde Ayrık Dalga Dönüşümü Algoritmasını kullanarak işlem yapar
EncoderMode.DCT4x4=4x4 bloklar şeklinde Ayrık Kosinüs Dönüşümü Algoritmasını kullanarak işlem yapar.
EncoderMode.DCT8x8=8x8 bloklar şeklinde Ayrık Kosinüs Dönüşümü Algoritmasını kullanarak işlem yapar.
EncoderMode.Lossless=%100 Gerçek kayıpsız sıkıştırma algoritmasını kullanır.
EncoderMode.Lossy=Hafif renk kaybıyla daha güçlü sıkıştırma yapan bir algoritmayı kullanır.
preencode:
Şimdilik 0 değerini versenizde olur
gray:true değeri için siyah/beyaz kayıt yapar false değeri için renkli

.hgf dosyalarını açmak için;
HGFComp hgfc=new HGFComp();
Bitmap resim= hgfc.DecompressPicture(".hgf dosyasının bulunduğu dizin");
Daha fazla bilgi için özelden mesaj atabilirsiniz face adresim;
https://www.facebook.com/RadioactiveZ

Eng
C # vs.. For use in projects, the HGFManager is now in the form of .dll;

CompressPicture (System.Drawing.Bitmap, [string], [int], [HGFCompressor.HGFComp.EncoderMode], [byte], [bool])
You can convert your bitmap image to .hgf.
Sample Usage
HGFComp hgfc = new HGFComp ();
hgfc.CompressPicture (Bitmap to be converted to Image, String FileName, int quality, EncoderMode encoder, byte display code, bool gray);
direct
As can be written as hgfc.CompressPicture (Bitmap to be converted to Image, String FileName);
Since the parameters are more professional;
Parameters:
Quality: Quality adjustment
encodermode:
EncoderMode.DWT32x32 = 32x32 blocks Discrete Wave Transformation
EncoderMode.DCT4x4 = 4x4 blocks Discrete Cosine Transform Processes by making algorithms.
EncoderMode.DCT8x8 = 8x8 blocks in discrete Cosine Transform Algorithm.
EncoderMode.Lossless = 100% Sets the true lossless technological algorithm.
EncoderMode.Lossy = Contains an algorithm that makes it stronger with slight color loss.
In preencoder:
If you give it a value of 0 for now
gray: true value for black / white records false value for color

To open the .hgf file;
HGFComp hgfc = new HGFComp ();
Bitmap image = hgfc.DecompressPicture (".hgf directory");
Private message for more information
https://www.facebook.com/radioactivez
