# �����ҤW���D��


-----------------------------------------------------
## �Ĥ@�D
* �]�w ver �ܼơA���e���y my kernel version is 3.xx �z�A�䤤 3.xx �� uname -r ��X����T�A����ܥXver�ܼƪ��ȡC(10%)


  1. ver="my kernel version is 3.xx"
  2. echo $ver��ܥXver�ܼƪ���
> my kernel version is 3.xx

  3. ver="my kernel version is 3.xx" uname -r
> 3.10.0-862.e17.x86_64


![image]()


* ����ܥثePATH�����ܼƪ��Ȭ���A�û���PATH���\�ά���? (10%)

  1. /usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin:/root/bin
  2. PATH���\��:
    * �@�~�t�η|�̷�PATH�����ܼƤ��ҳ]�w�����|���ǡA�̧ǴM��Ӹ��|�U�O�_���ĨϥΪ����O�C
    * �Y�䤣��A�N�|���command not found�C
    * ���h�ӥؿ��U�������O�A�H�u���䪺���D�C  


![image]()

-----------------------------------------------------
## �ĤG�D
* ���@���ɮת��ݩ��v���� drwxrwsr-x 3 root mail 4096 2�� 16 2017 mail/�A�л������ɮת��S�ʡC(10%)


���ɮ�mail�A�v��:rwx` (user�iŪ�i�g�i����) ` rws` (group�iŪ�i�g�i����A�B��SGID���v���A����̥i�Ȯɾ֦��ӵ{��mail�s�ժ��v��) ` r-x` (other�iŪ�i����) `�Auser��root�Agroup��mail�A�e�q��4096�A�̫�������2017/02/16�C


* ���]���@��script.sh�ɮת��v����-rw-r--r--�A�Y�Ʊ����Ҧ��H�i�H������ɮסA�аݸӦp��U�F���O�H�ШϥμƦr�k�P�Ÿ��k�U�ާ@�@���C(10%)


  * �Ʀr�k:chmod 755 script.sh
  * �Ÿ��k:chmod u=rwx,g=r-x,o=r-x script.sh

-----------------------------------------------------
## �ĤT�D
* ��������s���P�Ÿ��s�����t���C(10%)

  1. ����s��:�إߪ��C���ɮ׷|�e�Τ@��inode�A�ɮפ��e��inode�������ӫ��V�F�Ÿ��s��:�ҫإߪ��ɮ׬��@�ӿW�ߪ��s���ɮסA�|�e�Τ@��inode�Mblock�C
  2. ����s��:�N����@��**�ɦW**�R���Ainode�Mblock���٬O�s�b�F�Ÿ��s��:�ت��ɮ׳Q�R����A�]���䤣���l�ɦW�A�ҥHlink�|�ܦ���link�A�ӵL�k�}���ɮסC
  3. ����s��:������h�F�Ÿ��s��:������֡A�@��`�ϥΡC
  4. ����s��:�Y�Q�nŪ�����ɮסA�����n�g�L�ؿ��������ɦW�ӫ��V���T��inode���X�~��Ū���F�Ÿ��s��:���@�ӿW�ߪ��ɮסA�o�ӿW�ߪ��ɮ׷|���V�ت��ɮסA����Ū���ɡA�|���V�Llink�������ɮת��ɦW�C


* �b�a�ؿ��U�إߤ@���ɦW�� hosts.real ������s������ /etc/hosts�H (�Хά۹���|��ܮa�ؿ�) (5%)

  1. ` ln /home/hosts.real /etc/hosts `:�إ߹���s���C
  2. �۹���|:/home/hosts.real cd ../etc/hosts

* �b�a�ؿ��U�إߤ@���ɦW�� hosts.symbo ���Ÿ��s������ /etc/hosts�H (�Хά۹���|��ܮa�ؿ� (5%)

  1. ` ln -s /home/hosts.symbo /etc/hosts `:�إ߲Ÿ��s���C(/etc/hosts -> /home/hosts.symbo)
  2. �۹���|:/home/etc/hosts cd ../home/hosts.symbo


-----------------------------------------------------
## �ĥ|�D

