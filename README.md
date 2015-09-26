# Tim-hieu-cach-su-dung-VMWare-WorkStation


VMWare WorkStation là một hypervisor chạy trên máy tính x86-64, nó cho phép người dùng thiết lập một hoặc nhiều máy ảo trên một máy vật lý duy nhất, và sử dụng chúng đồng thời với các máy thực tế. Mỗi máy ảo có thể thực hiện riêng hệ điều hành, bao gồm cả các phiên bản của Microsoft Windows, Linux, BSD và MS-DOS. VMware WorkStation được phát triển và bán ra bới VMware Inc một bộ phận của tập đoàn EMC.


#1. Các tiện ích mà VMWare cung cấp

<img src="http://i.imgur.com/dAXbE5U.png">

- Khi mở VMWare WorkStation lên, bạn sẽ có 4 option để lựa chọn:
<ul>
<li>Create a New Virtual Machine<li/>
<li>Open a Virtual Machine</li>
<li>Connect to a Remote Server</li>
<li>Connect to VMware vCloud Air</li>
</ul>

##1.1 Create a New Virtual Machine( Tạo một máy ảo mới).

<img src="http://i.imgur.com/RuneMJL.png">

- Khi bạn chọn Create a New Virtual Machine sẽ có 2 option để bạn lựa chọn:
<ul>
<li>Typical</li>
<li>Custom</li>
</ul>

- Với lựa chọn Typical: (Được nhà cung cấp khuyên dùng) Bạn sẽ tạo ra máy ảo WorkStation 11.0 chỉ sau vài bước đơn giản.
- Với lựa chọn Custom: (Với nhiều tính năng nâng cao hơn) Có thể tạo ra máy ảo với khẳ năng tương thích với nhiều phiên bản VMWare trước đó chứ không chỉ là bản VMWare 11.0 như chế độ Typical.

Ở đây để đơn giản mình sẽ hướng dẫn ở chế độ lựa chọn Typical

- Sau khi chọn chế độ Typical và ấn next ta đến bước 

<img src="http://i.imgur.com/qHyitdo.png">

- Như đã biết máy ảo tạo ra cũng giống với máy tính vật lý, nó cũng cần có 1 hệ điều hành của riêng nó, để cài 1 hệ điều hành hiện tại có 2 lưa chọn, cài bằng đĩa và burn file iso ra usb sau đó boot vào máy tính vật lý. Ở đây VMWare cũng cung cấp cho người dùng những tùy chọn như vậy:
<ul>Install from:
<li>Installer disc(cài bằng đĩa CD)</li>
<li>Installer disc image file(iso)(cài bằng file iso)</li>
<li>Cài đặt hệ điều hành sau, máy ảo được tạo ra với một ổ đĩa trống.</li>
</ul>

- ở đây mình chọn như mặc định, và ấn next.

<img src="http://i.imgur.com/FXNYO94.png">

Như đã nói ở trên VMWare có thể cài đặt máy ảo với nhiều hệ điều hành thông dụng hiện nay như:
<ul>
<li>Microsoft Windows</li>
<li>Linux</li>
<li>Novell Netware</li>
<li>Solaris</li>
<li>VMWare ESX</li>
<li>Other</li>
</ul>

Ở đây chọ một hệ điều hành mà bạn muốn và chọn next.

<img src="http://i.imgur.com/uYPbvWQ.png">

Sau đó bạn chọn tên máy ảo và vị trí chứa tất cả các file cài đặt mà VMWare WorkStation tạo ra và ấn next.

<img src="http://i.imgur.com/iEdCOUK.png">

ở đây cho phép lựa chọn dung lượng tối đa mà ổ cứng chứa, có 2 tùy chọn cho việc lưu trữ:
<ul>
<li>Store virtual disk as a single file(Đối với tùy chọn này, sẽ lưu trữ ổ đĩa ở chỉ trong 1 file)</li>
<li>Split virtual disk into munltiple files(Đối với tùy chọn này, sẽ chia ổ đĩa ảo ra làm nhiều file, việc này thích hợp cho việc muốn chuyển ổ đĩa ảo đến 1 vị trí nào khác, vì khi ổ đĩa ảo được tạo ra có thể dung lượng nó sẽ rất lớn sẽ khó vận chuyển hơn)</li>
</ul>

Ở đây nên chọn Store virtual disk as a single file, vì đối với các loại ổ cứng di động hiện thời, hoàn toàn có thể di chuyển file 1 cách dễ dàng chứ không hoàn toàn cần phải chia nhỏ ra. Sau đó chọn Next

<img src="http://i.imgur.com/1ab23TR.png">

Đến bước này gần như máy ảo đã gần hoàn thiện, tuy nhiên có thể thay đổi các tùy chọn mặc định như ram, cpu, card mạng của máy ảo, bạn chọn Customize Hardware.

###Memory

<img src="http://i.imgur.com/TjNbXc6.png">

- Có thể lựa chọn Ram mà mình mong muốn.

- Màu xanh da trời chỉ dung lượng ram lớn nhất VMware cho phép(Dù là máy ảo nhwung ram cũng phải dựa trên của ram máy thật, bạn nên chọn dung lượng ram ở mức phù hợp trường hợp máy ảo của bạn dùng hết số lượng ram của máy thật sẽ dễ dẫn đến treo máy, dù cho nhà sản xuất vẫn cho bạn lựa chọ mức ram đó).
- Mầu xanh lá cây dung lượng Ram mà VMWare khuyên dùng là hợp lý.
- Mầu vàng dung lượng ram nhỏ nhất mà VMWare khuyên dùng.

###Processors.

<img src="http://i.imgur.com/dgyXyhB.png">

###New CD/DVD(SATA).

<img src="http://i.imgur.com/oVcGZJr.png">

- Cho phép đưa đĩa CD vào cấu hình hoặc dùng file iso để cấu hình.

<img src="http://i.imgur.com/UJFGkPs.png">

- Brower đến file iso muốn cấu hình

###Nework Adapter.

<img src="http://i.imgur.com/oc09ewI.png">

- Bridge: chế độ này như là một card mạng thật kết nối trực tiếp, nằm trong dải mạng cùng với máy thật.
- NAT: Tạo ra một địa chỉ IP ảo để máy ảo có thể kết nối ra ngoài, nó sẽ dịch chuyển địa chỉ IP ảo ra nằm cùng dải với địa chỉ IP của máy thật.
- Host Only: Để các máy ảo nằm trong cùng một switch ảo và kết nối ra ngoài

###USB Controller.

<img src="http://i.imgur.com/k4aQbdT.png">

###Sound Card.

<img src="http://i.imgur.com/b0XAzY2.png">

###Printer.

<img src="http://i.imgur.com/CI41sqO.png">

###Display.

<img src="http://i.imgur.com/FsDu2ZG.png">


##Ngoài ra VMWare WorkStation còn cung cấp chế độ Snapshot và chế độ Clone

- SNAPSHOT: lưu lại cấu hình từ lúc bạn chọn Take Snapshot đến trước
- Clone: Khi bạn muốn cấu hình nhiều máy dùng Win 7, bạn sẽ phải cấu hình từng máy một, tuy nhiên, VMWare WorkStation cho phép bạn Clone ra nhiều máy, bạn có thể thắc mắc là nếu bạn copy file cấu hình ra thì sẽ được chứ sao phải tạo ra bằng Clone. Tuy nhiên với mỗi máy bạn tạo ra bằng VMWare, chương trình sẽ tạo ra cho mỗi máy một địa chỉ Mac ảo duy nhất, nếu bạn copy thì sẽ tạo ra 2 máy có cùng 1 địa chỉ Mac, nếu bạn dùng Clone bạn sẽ tạo ra được nhiều máy ảo dùng cùng 1 hệ điều hành như nhau mà lại cod dịa chỉ Mac khác nhau.


#2. Demo hướng dẫn cài đặt ubuntu server 14.04 với VMWare WorkStation 11
http://i.imgur.com/fE0piAS.png
http://i.imgur.com/rztzTdn.png
http://i.imgur.com/VebkU3h.png
http://i.imgur.com/5kixR98.png
http://i.imgur.com/UZOH3GK.png
http://i.imgur.com/Ea1B2pQ.png
http://i.imgur.com/HKP88pH.png
http://i.imgur.com/Bt4f8Ut.png
http://i.imgur.com/WAwUUPC.png
http://i.imgur.com/IV6ZXOT.png
http://i.imgur.com/pgEHKC0.png
http://i.imgur.com/Mv6d8Jo.png
http://i.imgur.com/9BbxzEk.png
http://i.imgur.com/6PPrXDw.png
http://i.imgur.com/0aTHyZ5.png
http://i.imgur.com/5aCNRjE.png
http://i.imgur.com/d4yV9ga.png
http://i.imgur.com/JRPOYBs.png
http://i.imgur.com/WMRM1Rq.png
http://i.imgur.com/fmvlH5T.png
http://i.imgur.com/i8Ts3ll.png
http://i.imgur.com/9PQTQb9.png
http://i.imgur.com/vi1s7Ln.png
http://i.imgur.com/muEddU2.png
http://i.imgur.com/ddj2WuX.png
http://i.imgur.com/Mo0SGkO.png
http://i.imgur.com/SCQ4ct8.png
http://i.imgur.com/Vg4OB4U.png
http://i.imgur.com/9yX8alP.png
http://i.imgur.com/0boasBN.png
http://i.imgur.com/4thWr1d.png
http://i.imgur.com/crGfk4M.png
