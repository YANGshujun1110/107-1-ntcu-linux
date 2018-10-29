# HW4
==================================
## 1.�޲z�s�զ@�θ�ƪ��v���]�p:


* (1)�إ߸s�զW��:
  * �Q��**groupadd**�إ߸s��:mygroup�Bnogroup�C
> **grep**:�F�Ѩt�Τ��O�_�s�b�Q�n�d�ߪ��s�աC

> �t�Ϊ��s�ճ��O���b`` /etc/group ``�ɮ׸̡A�ҥH�d�ߪ��ɭԭn�O�o�[�W`` /etc/group ``��������|��!


![image]()
----------------------------------
* (2)�إ߱b���W��:
  * myuser1�Bmyuser2�Bmyuser3(**�ҥ[�Jmygroup�A�B�K�X�Ҭ�MyPassWord**)
> **useradd -G mygroup �b���W��**
> > **-G**:�᭱�|���۸s�զW�١A�̫�A���ۭn�[�J�s�ժ��b���C���~�A���]�|�ק�`` etc/group ``����������ơC

>�Q��**passwd �b���W��**���b���]�߱K�X�C

>�Q��**id �b���W��**�d�ݱb���̫�O�_���[�J**mygroup**���s�դ��C


![image]()
![image]()
![image]()
----------------------------------
* (3)�إ߱b���W��:
  * nouser1�Bnouser2�Bnouser3(**�ҥ[�Jnogroup�A�B�K�X�Ҭ�MyPassWord**)
> **useradd -G nogroup �b���W��**
> > **-G**:�᭱�|���۸s�զW�١A�̫�A���ۭn�[�J�s�ժ��b���C���~�A���]�|�ק�`` etc/group ``����������ơC

> �Q��**passwd �b���W��**���b���]�߱K�X�C

> �Q��**id �b���W��**�d�ݱb���̫�O�_���[�J**nogroup**���s�դ��C


![image]()
![image]()
![image]()
----------------------------------
* (4)�إߤ@�ӥؿ�`` /srv/myproject ``�A���ؿ��i�H��**mygroup**�s�դ����ϥΪ̧���ϥΡA�B`` �s�ت��ɮ׾֦��s�� ``��**mygroup**�A*��L�H�S�������v��*�C
  * �����ؿ��i�Jsrv�A�æb�䤤�إ�**myproject**��Ƨ��C
> **mkdir ��Ƨ��W��**:�إ߸�Ƨ��C


  * ����**ll**�d�ݭ�l�v���A��"drwxr-xr-x"�C
  * �Q��**chmod**�ק��v���A�O�o�̫�n�[�W��Ƨ��W�ٳ�C
  * �A�Q��**ll**�d�ݷ|�o�{�v���ק令�\�o�A��"drwxrwx---"�C
  * �Q��**chgrp mygroup myproject**�ק���ݪ��s�աA�A�Q��**ll**�d�ݴN�|�o�{���ݸs�դw�ܦ�mygroup�o�C
![image]()
----------------------------------
* (5)�Ȯɤ�������**myuser1**�������A�ëe��`` /srv/myproject ``�ؿ��A���իإߤ@�ӦW��`` myuser1.data ``���ɮסA����n�X**myuser1**�C
  * �����b����**myuser1**�C
  * ������`` /srv/myproject ``�ؿ��C
  * �Q��**touch myuser1.data**�b�䤤�إ߷s�ɮסC
> **touch**:�׭q�ɮת�����P�ɶ��A�åB�]�i�H�إߤ@�ӪŪ��ɮסC

  * �̫�n�X**myuser1**�C
![image]()
----------------------------------
* (6)�ƻs`` /usr/bin/ls ``��`` /usr/local/bin/myls ``��A�����ާ@:
  * �Q��**cp**�N`` /usr/bin/ls ``�ƻs��`` /usr/local/bin/myls ``�C
![image]()
  * �n�J**nogroup**�����䤤�@��(nouser1)�A���Q��**ll**�d��`` /usr/bin/ls ``�M`` /usr/local/bin/myls ``����T�A�|�o�{�o���Ӥ@�˪���T�C
  * ���@�}�l�٨S��k�d�ߨ�`` myls /srv/myproject ``(Permission denied)�C
![image]()
  * �����^**root**�ק��v��(**chmod u+s �ɮצW��**)�C
> **chmod u+s �ɮצW��**:�Ÿ��k�����ɮװ����v��(SUID)�C
> > SUID���v���X�Ь�Linux�ǲΤT�Ө������v���~���ĥ|���v���C
> > > ����̹��ӵ{���ݭn�㦳 x ���i�����v���ɡA�i�ϥΦ���k������̼Ȯɾ֦��ӵ{��mygroup�s�ժ��v���C

  * ���Q��**ll**�d���v����T�A�N�|�o�{�v���w�ק令�\�o�A��-rw**s**r-xr-x�C
  * �̫�����b����**nouser1**�A�d��`` myls /srv/myproject ``�A�N�i�H�d�ߨ�̭����ɮ׸�T(myuser1.data)�F�C
![image]()
=================================
## 2.�ϥε{���[����O�A�f�t**grep**������r�d�ߥ\��A�N��쪺**rsyslog**�������{�Ǫ� PID, PRI, NI, COMMAND ����T��s��`` /root/process_syslog.txt ``�ɮפ��C(�f�t`` > ``���ɦV��X)


* �Q������r�d�ߥ\��`` ps aux | grep rsyslog``���{���[��C
> **ps aux**:�˵�������process���p�C
> **grep �ɮצW��**:��M�æL�X�ɮפ��t���r��Ҧb�椺�e�C

* �ϥ�`` ps aux | grep rsyslog > /root/process_syslog.txt ``�N**rsyslog**�����{�Ǫ���T��s��**/root/process_syslog.txt**�C
* �A�Q��`` cat /root/process syslog.txt ``���ɮת����e�C�X��ù��W�C
> **cat**:�C�X�ɮפ��e�ܿù��W(�зǿ�X)�ΦX�֦h���ɮסC

![image]()
* ��J**top**��M**rsyslog**��PID�BPRI�BNI�BCOMMAND����T�C
> **top**:���ܥثe�t�ΪA�ȶ��ت��ʺA��ơC

  * PID��932�C
  * PRI��20�C
  * NI��0�C
  * COMMAND��rsyslogd�C
![image]()
=================================
## 3.�ϥ�**find**��X`` /usr/bin ``��`` /usr/sbin ``��ӥؿ����A�t��**SUID**���S���ɮ��ɦW�A�èϥ�**ls -l**�h�C�X��쪺�ɮת������v����A�N�ù������s��`` /root/findsuidsgid.txt ``�ɮפ��C(�ۦ�d��**find**���O�Ϊk�A�H�Ψϳz�L���ɦV�Ÿ�`` > ``��X�ɮ�)


* �ϥ�`` find /usr/bin /usr/sbin -perm /4000 ``��X����ӥؿ����t��SUID���S���ɮ��ɦW(�p��)�C
> `` find �ɮ� -perm /u=s ``:�C�L�X�t�Τ��Ҧ�SUID���ɮסC
> > **find**:�N�Q�n�M�䪺�ɮק�X�ӡC
> > **-perm**:�i�H���w�ɮת��v���C

![image]()
* `` find /usr/bin /usr/sbin -perm /4000 -exec ls -l {} \; > /root/findsuidsgid.txt ``�A�C�X�ɮת������v���C
> **-exec ���O {} \**:�i�H���ڭ̱N�j�M�X�Ӫ����G�A�ϥΨ�L�����O�i����򪺳B�z�ʧ@�C

![image]()
![image]()
![image]()