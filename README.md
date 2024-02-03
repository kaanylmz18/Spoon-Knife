### Well hello there!

Git bir versiyon kontrol sistemidir.(vks)
Diğer vksler delta-bazlı(değişim bazlı) olarak çalışırken git anlık görünüm referansları alarak çalışır.
Git dosyların sağlamasını yapmak için SHA-1 adında bir mekanizma kullanır.
Git dosyaları 3 ana durumda bulunabilir:

-> Modified, dosyayı değiştirdiğinizi ama henüz veritabanına commitlemediğinizi gösterir.
->  Staged, değiştirilmiş bir dosyayı bir sonraki commit anlık görünümünde işlenecek şekilde işaretlediğinizi gösterir.
-> Committed, dosyanın güvenli bir şekilde yerel veritabanınızda saklandığını gösterir.

Git’in iş akışı basitçe şöyledir:

1) Working tree’de dosyaları düzenlersiniz.
2) Bir sonraki committe işlenecek olan değişiklikleri seçersiniz.
3) Bir commit yaparsınız, staging area’daki dosyaların anlık görünümünü çeker ve Git klasörünüzde kalıcı olarak saklarsınız.

"git config --list" komutunu kullanarak Git’in o aşamada bulabildiği tüm ayarları listelemesini sağlayabilirsiniz.
"git help" yardım

"git init" komutu ile proje dosayısının olduğu yerde repository oluşturulur.
"git clone <url>" komutu ile var olan bir proje repository olarak alınır.
"git status" komutu ile dosyalarının durumu kontrol edilir
"git status -s" dosyalarının durumu özet bir şekilde gösterilir
"git add <files>" komutu ile takip edilicek dosyalara yeni bir tanesi eklenir
".gitgnore" ile takip edilmek istenmeyen dosyalar belirtilebilir.
"git diff" ile değişiklik yapılan ve unstaged olan dosyaların bilgisi görüntülenir.
"git commit -m ''" ile yapılan değişiklikler commit edilir.
"git commit -a -m ''"  '-a' ile stage are skiplenebilir.
"git rm" ile istenilen dosya remove edilebilir.
"git log" ile commit history görüntülenebilir.
"git fetch" ile hedefteki dosyalar toplanır.
"git push" ile yapılan değişiklikler servera iletilir.
"git branch <branchname>" ile yeni bir branch oluşturulur.
"git checkout <branchname>" ile çalışılan branch değiştirilebilir.
"git merge" ile branchler birleştirilebilir.
