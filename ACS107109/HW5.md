# HW5
---------------------------------
## ����s���ɮת��ظm�欰:


---------------------------------
### �b /etc/hosts �ɮסA�Ч�X


> �Q��`` ls -ali �ɮצW��  ``��Minode���X�C
> > **ls -ali**�̫e�����ƭȧY��inode���X�C
> > > **-a**:�������ɮסA�s�P������( �}�Y�� . ���ɮ�) �@�_�C�X�ӡC
> > > **-l**:����Ʀ�C�X�A�]�t�ɮת��ݩʻP�v��������ơC
> > > **-i**:�C�X inode ���X�C
> > > > **-ali**��**-a**�B**-l**�B**-i**���զX�C


* ���ɮת� inode ���X���X���H


**2129800**


* �o�� inode �@���X���ɦW�b�ϥΡH


**1**


![image]()


---------------------------------
### �إ߹���s���A��l�ɮ׬� /etc/hosts �ӷs���ɮ��ɦW�� /srv/hosts.hard�A�Ч�X


> �Q��`` ln /etc/hosts /srv/hosts.hard ``�إ߹���s���C
> > **ln ����ؿ����ɮ� �s�����ؿ����ɮ�**:�s���ɮשΥؿ��C
> > > �N`` /etc/hosts ``�s����`` /srv/hosts.hard ``�C

> �A�Q��`` ll -i /etc/hosts /srv/hosts.hard ``�d���ɮ׬�����T�C
> > **-i**:�C�X inode ���X�C
> > > �|�o�{�����ɮצW�٨ϥΦP�@��inode���X(�s����:2)�C


* /srv/hosts.hard�� inode ���X���X���H


**2129800**


* �o�� inode �@���X���ɦW�b�ϥΡH


**2**


![image]()


* ������]


�]���C�ӥؿ����U����`` . ``���ɮצW�١A�åB`` . ``�S�N���ؿ��ۤv�A�ҥH**�ؿ������|������ɮצW�ٸ��H�ۤv**�A�Ϥ��A**�|������ɮצW�ٳs���ܬۦP��inode���X**�C
> �]���A��inode���X�|������ɮצW�٦b�ϥΡC

> **hard link**
> >�C���ɮ׳��|�ϥΤ@��inode�A�ɮת����e��inode���O���ӫ��V�C�]���A�Q�nŪ�����ɮ׮ɡA���g�ѥؿ��O�����ɮצW�٫��V���T��inode���X�~�i�HŪ���C
> > > �h���ɮצW�٥i�H������P�@��inode���X�C

> **inode �P block ���S�����ܡC**


![image]()


---------------------------------
### �إ߲Ÿ��s���A��l�ɮ׬� /etc/hosts �ӷs���ɮ��ɦW�� /srv/hosts.soft�A�Ч�X


> �Q��`` ln -s /etc/hosts /srv/hosts.soft ``�إ�Symbolic link�C
> > **ln -s �u��ؿ����ɮ� �s�����ؿ����ɮ� ``:�s���ɮשΥؿ��C
> > > **-s**:���� symbolic line ���s���C
> > > > �N`` /etc/hosts ``�s����`` /srv/hosts.soft ``�C

> **�P�Ĥ@�D���B�J�d��inode���X�H�Φ@���X���ɦW�b�ϥ�**�C
> > �Q��`` ls -ali �ɮצW��  ``��Minode���X�C
> > > **ls -ali**�̫e�����ƭȧY��inode���X�C
> > > > **-a**:�������ɮסA�s�P������( �}�Y�� . ���ɮ�) �@�_�C�X�ӡC
> > > > **-l**:����Ʀ�C�X�A�]�t�ɮת��ݩʻP�v��������ơC
> > > > **-i**:�C�X inode ���X�C
> > > > > **-ali**��**-a**�B**-l**�B**-i**���զX�C


* /srv/hosts.soft�� inode ���X���X���H


**309227**


* �o�� inode �@���X���ɦW�b�ϥ�


**1**


![image]()


* ������]


�]���䬰�إ�**��@���W�߷s�ɮ�**�A�B���ɮ׷|��**���Ū���ɪ������V��link�����ɮפ��e**�C
> �]���A��inode���X�u�|���@���ɮצW�٦b�ϥΡC

> **symbolic link**

> **inode �P block �|���ܡC**
> >�|���α� inode �P block�C


-----------------------------------------
####�ɥR:


* �ѩ�C�@�x�q�������P�A�ҥH�C�ӤH��inode���X�|���Ӥ@�ˡC
* �p�Gln���[����ѼơA��N�ݩ����s��(hard link)�C