# LIBREBOOT

**Libreboot - это свободная замена проприетарному загрузочному коду BIOS/UEFI, которая уважает Вашу свободу.** 

Загрузочный код исполняется в тот момент, когда Вы включаете компьютер. Это код низкого уровня, используемый для инициализации "железа" компьютера и создания условий для запуска операционной системы. 

Обычно для этого используются прошивки BIOS/UEFI, которые содержат закрытый код и бэкдоры, зачастую с зашифрованными участками. Не имея доступа к исходному коду низкого уровня, запускающего Ваш компьютер, Вы не можете знать, что именно этот код делает и тем самым добровольно (ведь Вы платите за железо, а не Вам платят за то, чтобы Вы его использовали) лишаете себя свободы. 

Особенно актуально это стало после всеобщего внедрения технологии Intel Active Management Technology и её аналога от AMD, которые обеспечивают возможность дистанционного управления Вашим компьютером и имеют независимый от операционной системы доступ к оперативной памяти, сетевым подключениям и жестким дискам Вашего компьютера вне зависимости от того, включен он или нет. Доступ осуществляется по независимому каналу TCP/IP, а сам закрытый и зашифрованный код системы хранится на флеш-памяти, встроенной в чип BIOS, и исполняется встроенным микропроцессором независимо от центрального. См. [https://ru.wikipedia.org/wiki/Active_Management_Technology](https://ru.wikipedia.org/wiki/Active_Management_Technology). Несмотря на многочисленные попытки, расшифровать закрытый код подобных систем от Intel и AMD до сих пор не удалось, а попытки обхода системы оказывались (за немногими исключениеми) неудачными.

Широкое внедрение описанной выше технологии началось с 2008 года, а уже с 2009-2010 годов подавляющее большинство материнских плат настольных систем и ноутбуков выпускаются исключительно с её применением. 

**Libreboot-это [полностью свободное программное обеспечение](https://www.gnu.org/philosophy/free-sw.html), в которое каждый может внести свой вклад или проверить его исходный код.** Libreboot распространяется на основании принципов [Copyleft](http://www.gnu.org/licenses/copyleft.html), то есть (по большей части) по лицензиям [GNU General Public License v2 и v3](http://www.gnu.org/licenses/gpl.html). Это означает, что Libreboot всегда будет бесплатным для всех. Если бы кто-то взял Libreboot и попытался сделать его собственностью, он бы нарушил закон. Принцип Copyleft подразумевает, что Libreboot - это общественное достояние: знания и власть распространяются без какой-либо дискриминации.

**Libreboot работает быстрее, безопаснее и надежнее, чем большинство несвободных прошивок.** Libreboot предоставляет множество дополнительных функций, таких как шифрование загрузки, проверка подписи GPG перед загрузкой ядра Linux и многое другое!

Libreboot основан на [coreboot](https://www.coreboot.org/) и не содержит bloobs (кусков двоичного кода). Философия проекта: сделать бесплатное загрузочное микропрограммное обеспечение доступным для всех. Другими словами, Libreboot - это дистрибутив coreboot, который объединяет все необходимые программные компоненты в единый унифицированный пакет.

# Почему я должен использовать Libreboot?

Ниже дословный перевод обращения сообщества Libreboot с официального сайта проекта [https://libreboot.org/](https://libreboot.org/):

> А ты знал, что у тебя есть права? Право на неприкосновенность частной жизни, свободу мысли, свободу слова и право на чтение. В контексте вычислительной техники это означает, что любой человек может использовать [свободное программное обеспечение](https://www.gnu.org/philosophy/free-sw.html). Проще говоря, свободное программное обеспечение - это программное обеспечение, находящееся под прямым суверенитетом пользователя и, что более важно, коллектива, то есть сообщества. 

Несвободные программы (например, Windows, MacOS или проприетарные BIOS/UEFI) находятся под исключительным контролем их владельцев, а не пользователей! С помощью уважающего свободу программного обеспечения пользователи могут в любое время изучить исходный код и даже сами стать разработчиками! Хотите помочь делу? Некоторые способы внести свой вклад могут заключаться в написании документации, предоставлении поддержки пользователям или тестировании вклада других пользователей. Вам нужно больше идей о том, как вы можете помочь с проектом? Если вы хотите, чтобы была разработана конкретная функция, но у вас нет технической склонности, вы можете нанять любого, кто будет выполнять эту работу за вас. С помощью свободного программного обеспечения вы, по сути, являетесь владельцем своей собственной копии, поэтому она свободна.

Многие люди используют несвободные проприетарные загрузочные прошивки, даже если они используют GNU+Linux. Несвободная прошивка BIOS/UEFI часто содержит бэкдоры, может быть медленной и иметь серьезные ошибки. От разработки и поддержки можно отказаться в любой момент. Напротив, libreboot-это полностью свободное программное обеспечение, где каждый может внести свой вклад или проверить его код. Libreboot - это не просто свободное программное обеспечение; это также программное обеспечение авторского Лева, выпущенное под (По большей части) смесью GNU General Public License v2 и v3. Это означает, что программное обеспечение всегда будет бесплатным для всех. Если бы кто-то взял Libreboot и попытался сделать его собственностью, он бы нарушил закон. Другими словами, авторское лево обеспечивает общественное достояние, где все знания и власть делятся без какой-либо дискриминации.


## Основные ссылки

* [Официальный сайт проекта](https://libreboot.org).
* [Открытый репозиторий этого перевода. Примите участие!](https://github.com/Zoviet/libreboot)
* [IRC канал проекта.](https://webchat.freenode.net/?channels=libreboot)
* [Репозиторий и баг-трекер проекта.](https://notabug.org/libreboot/)
