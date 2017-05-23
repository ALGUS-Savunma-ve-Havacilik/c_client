GridDB C�N���C�A���g

## �T�v

GridDB C�N���C�A���g��C����p�̃C���^�t�F�[�X��񋟂��܂��B  
�܂��A���̃��|�W�g���ɂ͊ȒP�ȃT���v���v���O����������܂��B  
�ڍׂ�API���t�@�����X��API(C����)�̏͂��Q�Ƃ��Ă��������B

## �����

�ȉ��̊���C�N���C�A���g�̃r���h�ƃT���v���v���O�����̎��s���m�F���Ă��܂��B

    OS:             CentOS 7.3(x64)
    GCC:            Version 4.8.5
    GridDB server:  Version 3.0 CE(Community Edition)

## �N�C�b�N�X�^�[�g

### C�N���C�A���g�̃r���h

    $ cd client/c
    $ ./bootstrap.sh
    $ ./configure
    $ make 
    
�����s����ƁAbin�t�H���_�̉��Ɉȉ��̃t�@�C���⃊���N���쐬����܂��B

    libgridstore.so
	libgridstore.so.0
	libgridstore.so.0.0.0

### �T���v���v���O�����̎��s
���O��GridDB�T�[�o���N�����Ă����K�v������܂��B

    $ cp client/c/sample/sample1.c .
    $ gcc -I./client/c/include -L./bin sample1.c -lgridstore
    $ export LD_LIBRARY_PATH=${LD_LIBRARY_PATH}:./bin
    $ ./a.out <GridDB notification address(default is 239.0.0.1)> <GridDB notification port(default is 31999)>
      <GridDB cluster name> <GridDB user> <GridDB password>
      -->Person: name=name02 status=false count=2 lob=[65, 66, 67, 68, 69, 70, 71, 72, 73, 74]

��client/c/include�t�H���_�̉��ɁA�r���h�Ɏg����gridstore.h�t�@�C��������܂��B  
��client/c/sample�t�H���_�̉��ɁA�T���v���v���O����������܂��B

## �h�L�������g
  �ڍׂ͈ȉ��̃h�L�������g���Q�Ƃ��Ă��������B
  - [API���t�@�����X](https://griddb.github.io/griddb_nosql/manual/GridDB_API_Reference_ja.html)

## �R�~���j�e�B
  * Issues  
    ����A�s��񍐂�issue�@�\�������p���������B
  * PullRequest  
    GridDB Contributor License Agreement(CLA_rev1.1.pdf)�ɓ��ӂ��Ē����K�v������܂��B
    PullRequest�@�\�������p�̏ꍇ��GridDB Contributor License Agreement�ɓ��ӂ������̂Ƃ݂Ȃ��܂��B

## ���C�Z���X
  C�N���C�A���g�̃��C�Z���X��GNU Affero General Public License (AGPL)�ł��B  
  �T�[�h�p�[�e�B�̃\�[�X�ƃ��C�Z���X�ɂ��Ă�3rd_party/3rd_party.md���Q�Ƃ��������B
