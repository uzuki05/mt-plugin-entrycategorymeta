EntryCategoryMeta
===========

* Author:: Yuichi Takeuchi <uzuki05@takeyu-web.com>
* Website:: http://takeyu-web.com/
* Copyright:: Copyright 2012 Yuichi Takeuchi
* License:: MIT-LICENSE

�u���O�L���ƃJ�e�S���̊ԂɃ��^�f�[�^��ǉ��ł���悤�ɂȂ�܂��B
���̓t�H�[���̃e���v���[�g�������Őݒ�ł��A�ǉ����郁�^�f�[�^�̎��R�x�������̂������ł��B

����v��
-----------

MT(MTOS) 5.1

���̃o�[�W�����͕s���B

�C���X�g�[��
-----------

plugins/EntryCategoryMeta �� MT_DIR/plugins/ �ɃR�s�[���ĉ������B

�ݒ�
-----------

���^�f�[�^��ǉ����������u���O�̃v���O�C���ݒ肩��L���ɂ��A�t�H�[���e���v���[�g��ҏW���܂��B

�t�H�[���e���v���[�g�́A�ҏW��ʂ̃J�e�S���E�B�W�F�b�g�Ŏg�p�����ATemplate.js�e���v���[�g�ɖ��ߍ��܂�܂��B

  <select name="select1">
  <option value=""]></option>
  [# selected='' #][# if ( item.meta.select1 == "Apple" ) selected='selected' #]
  <option value="Apple" [#= selected #]>Apple</option>
  [# selected='' #][# if ( item.meta.select1 == "Orange" ) selected='selected' #]
  <option value="Orange" [#= selected #]>Orange</option>
  [# selected='' #][# if ( item.meta.select1 == "Banana" ) selected='selected' #]
  <option value="Banana" [#= selected #]>Banana</option>
  </select>
  <input type="text" name="text1" value="[#= item.meta.text1 #]" />


���p���@
-----------

�u���O�L���̕ҏW��ʂ̃J�e�S���E�B�W�F�b�g�ŁA�J�e�S�����Ƀt�H�[�����\������A���͂��ł���悤�ɂȂ�܂��B
�v���r���[�ɂ��Ή����Ă��܂��B


���^�f�[�^�̕\��
-----------

�ȉ��̃e���v���[�g�^�O���񋟂���܂��B
���ɁA�u�u���O�L���̃J�e�S���v�̃R���e�L�X�g�ŗ��p�ł��܂��B

### MTIfEntryCategoryMeta�R���f�B�V���i���^�O

�R���e�L�X�g�̃u���O�L���̃J�e�S���Ƃ̊ԂɃ��^�f�[�^���ݒ肳��Ă���΃u���b�N�������B

### MTEntryCategoryMeta�t�@���N�V�����^�O

name���f�B�t�@�C�A�Ŏw�肵�����O�̃��^�f�[�^�̒l���擾

### �T���v��

  <mt:EntryCategories>
    <a href="<$mt:CategoryArchiveLink$>" rel="tag" title="<$mt:CategoryDescription escape="html"$>"><$mt:CategoryLabel$></a>
    <mt:IfEntryCategoryMeta>
      <br />
      <$MTEntryCategoryMeta name="select1" escape="html"$><br />
      <$MTEntryCategoryMeta name="hour1" zero_pad="2"$>:<$MTEntryCategoryMeta name="min1" zero_pad="2"$>
      �`
      <$MTEntryCategoryMeta name="hour2" zero_pad="2"$>:<$MTEntryCategoryMeta name="min2" zero_pad="2"$>
    </mt:IfEntryCategoryMeta>
  </mt:EntryCategories>


����
-----------

�����p�͎��ȐӔC�ŁB
