apktool
=======

һ.������Apk�õ�JavaԴ���� 
ת���ԣ�http://hi.baidu.com/%CB%BF%D4%B5%CC%EC%CF%C2/blog/item/2284e2debafc541e495403ec.html
 
�������أ����õ�dex2jar��JD-GUI��2������
dex2jar���ص�ַ��http://laichao.googlecode.com/files/dex2jar-0.0.7-SNAPSHOT.zip
JD-GUI���ص�ַ��
  windows��JD-GUI��http://laichao.googlecode.com/files/jdgui.zip
  Linux��JD-GUI��http://laichao.googlecode.com/files/jd-gui-0.3.2.linux.i686.tar.gz
���裺
1.�����ҵ�Android�����װ���е�classes.dex
��.apk�ļ�����Ϊ.zip��Ȼ���ѹ��,�õ����е�classes.dex�ļ���������java�ļ�������ͨ��dx���ߴ���ɵ�,�����������Ǿ��������ᵽ��2���������淽�򵼳�javaԴ�ļ�

2.��classes.dex������dex2jar.bat����Ŀ¼��
��������ģʽ�¶�λ��dex2jar.bat����Ŀ¼������ dex2jar.bat classes.dex  ������classes.dex.dex2jar.jar 

3.����JD-GUI���ߣ�������ɫ���밲װ�ģ�
�������jar�ļ������ɿ���Դ����

---------------------------------------------------------------------------------
������apk���ɳ����Դ�����ͼƬ��XML���á�������Դ���ļ���

APKTool��GOOGLE�ṩ��APK���빤�ߣ���ҪJAVA���л������Ƽ�ʹ��JDK1.6����JDK1.7��
��������APK�ļ������޸ģ���ô�Ͳ��ɱ����Ҫʹ�õ�APKTool����̳���кܶ����ROM���������Ӷ���Ҫ�Լ������޸�APK�ļ��������޸�framework-res.apk��systemUI.apk�ȵȡ�
���Ÿ�λ�в����˿��˺����������޸�һ�������ǽ��ȴ�������˸�ʽ�����Ĵ���ȴ�޷����и�������������֪���Լ��������

һ��APKTOOLʹ�û�������
1.��װJAVA�����û���������
���ذ�װ���ܼ򵥣��ؼ��ǰ�װ�����Ҫ�������û��������Է������������ܹ�����JAVA��
��WIN7Ϊ�������������Ҽ�������������>���ԡ���>�߼�ϵͳ���á���>������������>���±ߵ�ϵͳ�������½�һ��������������ΪJAVA_HOME��ֵΪJAVA�İ�װ·���������ҵ���H:\ProgramFiles\Java\jdk1.6.0_26

����APKTool�İ�װ
1.��ʵ���̸���ϰ�װ�����������Ը��Ļ����԰����ص���APKTOOL�е������ļ���aapt.exe��apktool.bat��apktool.jar����ѹ�������Windows��װĿ¼�£��Է���ʹ��Dos����.
2.������Щ�����ص�APKTOOL���и���װ��bat�ļ���������������������ʹ�õ�bat�ļ����������Ҳ��Ƽ����ʹ����Щbat�ļ�����Ȼʹ�������ܷ��㣨��ʵ�Ҳ������÷��㣩������������ִ��󲻷���鿴��

����APKTool��ʹ��
1.decode
���������ڽ��з�����apk�ļ���һ���÷�Ϊ
apktool d <file.apk> <dir>
<file.apk>������Ҫ�������apk�ļ���·�������д����·��������C:\MusicPlayer.apk
<dir>�����˷��������ļ��Ĵ洢λ�ã�����C:\MusicPlayer
����������<dir>�Ѿ����ڣ���ô���������������ʾ�㣬�����޷�ִ�У���Ҫ�������޸��������-fָ��
apktool d �Cf <file.apk> <dir>
�����ͻ�ǿ�и����Ѿ����ڵ��ļ�

2.build
���������ڱ����޸ĺõ��ļ���һ���÷�Ϊ
apktool b <dir>
�����<dir>���Ǹղ��㷴����ʱ�����<dir>����C:\MusicPlayer��,����������������һ����������ᷢ��C:\MusicPlayer�ڶ���2���ļ���build��dist�����зֱ�洢�ű�����������������ļ��Լ����մ����apk�ļ���

3.install-framework
����������ΪAPKTool��װ�ض���framework-res.apk�ļ����Է�����з�����һЩ��ROM�໥������APK�ļ���

4.����������AndroidMenifest.xml
java -jar AXMLPrinter2.jar  AndroidManifest.xml  > newxml.xml

5.ʹ��AXMLPrinter2.jar����������xml�ļ�. ����Ҫ������layoutĿ¼�µ�����xml�ļ�, 
��Ҫ��AXMLPrinter2.jar��layout��ͬһ��Ŀ¼��, Ȼ���дbat�ű�: 
 for /r layout %a in (*.xml) do @java -jar AXMLPrinter2.jar "%a">>"%a".xml . ִ�����OK��. 
