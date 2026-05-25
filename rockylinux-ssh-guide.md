**Rocky Linux Setup on Oracle VirtualBox and SSH Connection via MobaXterm

This document provides a step-by-step guide on how to start a Rocky Linux virtual machine using Oracle VirtualBox and establish a secure SSH connection using the MobaXterm terminal client.

1. Starting the Virtual Machine
Open the Oracle VirtualBox Manager application.

Select the target virtual machine (rockylinux) from the list on the left panel.

Click the green Start button on the top menu to power on the operating system and bring it to the "Running" state.

2. Launching MobaXterm
Open the MobaXterm Personal Edition application.

Locate the pre-configured SSH session from the "User sessions" panel on the left or from the "Recent sessions" dashboard.

3. Establishing SSH Connection and Terminal Access
Double-click on the configured 127.0.0.1 (train) session to initiate the connection.

A secure SSH tunnel will be established to train@127.0.0.1 via local port forwarding.

After successful user authentication (entering credentials), access to the Rocky Linux terminal ([train@trainvm ~]$) is granted.

The system is successfully connected, and the Miniconda base environment is active and ready for package management and further operations.



**Oracle VirtualBox Üzerinde Rocky Linux Kurulumu ve MobaXterm ile SSH Bağlantısı
Bu doküman, Oracle VirtualBox üzerinde çalışan Rocky Linux sanal makinesinin başlatılması ve MobaXterm terminal istemcisi kullanılarak güvenli bir SSH bağlantısının nasıl kurulacağını adım adım açıklamaktadır.

1. Sanal Makinenin Başlatılması
Oracle VirtualBox Yöneticisi uygulamasını açın.

Sol panelde yer alan listeden ilgili sanal makineyi (rockylinux) seçin.

Üst menüde bulunan yeşil Başlat (Start) butonuna tıklayarak işletim sistemini "Çalışıyor" durumuna getirin.

2. MobaXterm İstemcisinin Hazırlanması
MobaXterm Personal Edition uygulamasını çalıştırın.

Sol taraftaki "User sessions" (Kullanıcı oturumları) panelinden veya ana ekrandaki "Recent sessions" (Son oturumlar) listesinden daha önce yapılandırılmış olan SSH oturumunu seçin.

3. SSH Bağlantısının Kurulması ve Terminal Erişimi
Yapılandırılmış olan 127.0.0.1 (train) oturumuna çift tıklayarak bağlantıyı başlatın.

Port yönlendirme (Port Forwarding) aracılığıyla train@127.0.0.1 adresine güvenli bir SSH tüneli kurulacaktır.

İlgili kullanıcı kimlik doğrulaması (şifre girişi) tamamlandıktan sonra Rocky Linux terminaline ([train@trainvm ~]$) başarıyla erişim sağlanır.

Sistem üzerinde Miniconda ortamı aktiftir ve temel paket yönetimi işlemleri için hazırdır.
