newentry �v���O�C���ɂ���

���T�v
�@newentry �v���O�C���́A������u�f���v�̃C���[�W�ŐV�����G���g����ǉ��ł���v���O�C���ł��Bblosxom ���x�[�X�Ɍf�����^�p���������Ɏg�p�ł��܂��B
�@�܂��A�G���g���ɑ΂��ăR�����g���������ꍇ�́A���ʂ̃u���O�̂悤�ɃG���g�������n��ɕ\������̂ł͂Ȃ��A�X���b�h�t���[�g�^�f���̂悤�ɁA�ŐV�̃R�����g�����������ԂɃG���g������בւ���@�\������܂��B

�@�O�ɍ�����o�[�W�����͂��܂�ɑ��@�\�����Đݒ肷��̂������e����̂��ʓ|�������̂ŁA�s�v�Ǝv����@�\���o�b�T������ď�L�̋@�\�݂̂ɍi��܂����B
�@�����A���ꂾ������΋@�\�Ƃ��Ă͏\�����Ǝv���܂��B


�����ӎ���
�@���̃v���O�C���̓���ɂ́A�ʓr writeback �v���O�C�����K�v�ł��B
�@�i�Ȃ��ƃG���g���ɑ΂���R�����g�̏������݂��ł��Ȃ��̂ŁA�f���ɂȂ�܂���j

�@�܂��A���̃v���O�C���́Akyo ���񐧍�� blosxom Starter Kit (�ȉ�"BSK") ���g�p���� blosxom ���C���X�g�[�����Ă��邱�Ƃ�O��Ƃ������ɂȂ��Ă��܂��B��̓I�ɂ́ABSK �� config.cgi �ɏ����ꂽ�Awriteback�v���O�C���̕ϐ��̒l���Q�Ƃ��Ă��܂��B
�@����BSK���g�킸��blosxom���^�p���Ă��鎞�́A�ʓr�v���O�C���̐ݒ肪�K�v�ɂȂ�܂��B

�@blosxom Starter Kit: http://hail2u.net/archives/bsk.html


���C���X�g�[���ƑO����
�@�𓀂���ƁA�ȉ��̃t�@�C�����o�Ă��܂��B

plugins
 newentry  �v���O�C���{��
           �v���O�C���̃f�B���N�g��(plugins)�ɐݒ肵�܂��B

entries
 newentry.html  ���̓t�H�[���̐��`�i�t�H�[���\�����ɂ͂����ǂݍ��݂܂��j
 writeback.html writeback �̓��e��ʏ펞�ɕ\�����邽�߂ɕK�v�ȃt���[�o�[�i�K���ɏC�����ĉ������j
                ���ꂼ��A�t���[�o�[�̃f�B���N�g��(entries)�ɐݒ肵�܂��B

�@���݂��g�p�ɂȂ��Ă���t���[�o�[�ɁA���L�̋L�q��K�X�ǉ����ĉ������B

$newentry::form         ���̓t�H�[����\���inewentry.html �̓��e��W�J���܂��j
$newentry::response     newentry ����̃��b�Z�[�W��\��
$newentry::date         �G���g���̍X�V����������istory �Ŏg�p�\�j
$writeback::writebacks  story.html �� $body �̉��ɖ��ߍ��ނ��Ƃɂ��A�G���g���ɑ΂���R�����g���iwriteback.html���K�p���ꂽ�`�Łj���̕����ɕ\�������悤�ɂȂ�܂��B���\�����f�����ۂ��B

�@�����āABlosxom�̃f�[�^�f�B���N�g��(entries)�ɁA�������݃t�@�C����ۑ�����p�̃f�B���N�g���i��Fbbs�j���쐬���ĉ������B
�@�����܂ł������Ԃ�blosxom���ĕ\������΁A���̓t�H�[�����o�Ă��Čf���Ƃ��Ďg�����ԂɂȂ��Ă���񂶂�Ȃ����Ǝv���܂��B�����B


���ݒ荀�ڂ̐���
�@�v���O�C���ׂ̍����ݒ�́A�v���O�C���̃\�[�X�̒��̕ϐ��������邱�Ƃɂ���čs���܂��B
�@���ʂ͂���Ȃɂ�����Ȃ��ėǂ��Ǝv���܂��B

# ���̃v���O�C���̖��O
$newentry_plugin_name = "newentry";
�@�t�H�[��������͂��ꂽ�ꍇ�A���̃v���O�C�������̏������݂��ǂ����𔻒f���邽�߂Ɏg�p���閼�́B
�@�ȉ��̋L�q���A�t�H�[���̒��ɕK������Ă����ĉ������B
�@<input type="hidden" name="plugin" value="newentry" />

# �G���g����ǉ�����f�t�H���g�̃f�B���N�g����
$newentry_category = "bbs";
�@�t�H�[��������͂��ꂽ�������݂�ۑ�����A$blosxom::data_dir �z���̃f�B���N�g���̖��O�B
�@�u�C���X�g�[���ƑO�����v�̎��ɍ쐬�����f�B���N�g���̖��O��ݒ肵�ĉ������B

# �쐬����t�@�C���̊g���q
$file_extension = $blosxom::file_extension;
�@�t�H�[��������͂��ꂽ�������݂�ۑ�����ۂɐݒ肷��g���q�B
�@�ʏ�͂��̂܂܂ŗǂ��ł��B

# ������R�����g�̃o�C�g���i�ő�j
$max_length_comment = 8096;
�@�������ݎ��̃R�����g�̍ő�o�C�g���B
�@���ɐ������Ȃ��ꍇ�́A0��ݒ肵�ĉ������B

# ������R�����g�̃o�C�g���i�ŏ��j
$min_length_comment = 40;
�@�������ݎ��̃R�����g�̍ŏ��o�C�g���B�ꌾ�R�����g���������̂����ȏꍇ�p�B
�@���ɐ������Ȃ��ꍇ�́A0��ݒ肵�ĉ������B

# ��������s�̐�
$denyret = 30;
�@���̓��e�̒��Ɋ܂܂����s�̐��̍ő�l�B�u�r�炵�v�΍�̈�B
�@���ɐ������Ȃ��ꍇ�́A0��ݒ肵�ĉ������B

# ����IP���狖���鏑�����݊Ԋu�i�b�j
$deny_timesrc = 60;
�@�����IP�A�h���X����̘A�����e���������ꍇ�A�����铊�e�Ԋu�̎w��B�u�r�炵�v�΍�̈�B
�@���ɐ������Ȃ��ꍇ�́A0��ݒ肵�ĉ������B

# �G���g���P�s�ڂ̃t�H�[�}�b�g
# $title: ���̓^�C�g�� / $name: ���O(URL��e-mail�ւ̃����N����)
# title ���Ȃ��ꍇ�A$name ���g�p����܂�
$format_first_line = '$title ($name)';
�@�t�H�[�����瓊�e���ꂽ�������݂̓t�@�C���Ƃ��ĕۑ�����܂����A����̂P�s�ڂ̃t�H�[�}�b�g�iblosxom�ł̓G���g���̃^�C�g���Ƃ݂Ȃ����j���w�肵�܂��B
�@url ���� URI �⃁�[���A�h���X�����͂���Ă����ꍇ�A$name �ɂ͂���ւ̃����N�������I�ɐݒ肳��܂��B

# Writeback���������G���g������ʂɎ����Ă���@�\�i������age�j���g�p�H
$use_age = 1;
�@���̕ϐ���0�ȊO�̏ꍇ�A�G���g���̍X�V�����́i�G���g�������e���ꂽ�����ł͂Ȃ��j���̃G���g���ɍŌ�� Writeback ���ꂽ���̎����Ƃ݂Ȃ��悤�ɂȂ�܂��B
�@���ʓI�ɁA�ŋ�Writeback ���������G���g���قǏ�ɕ\������܂��B

# �f�t�H���g�̃t�H�[��
my $def_form_template =<<'FORM_';
�i�����j
FORM_
�@�t���[�o�[�p�̃f�B���N�g���� "newentry.html" �Ƃ����t�@�C�����Ȃ��ꍇ�A�����ŏ����ꂽ�t�H�[�����g�p���܂��B

# �N�b�L�[
my $cookie_expires = $blosxom::writeback_cookie_expires;
my $cookie_domain = $blosxom::writeback_cookie_domain;
my $cookie_path = $blosxom::writeback_cookie_path;
�@���ꂼ��A�T�[�o�̃h���C���Ablosxom ��ݒu�����p�X�A�ۑ����Ԃ�ݒ肵�Ă��܂��B
�@$blosxom::writeback_�` �Ƃ����ϐ��� BSK �� config.cgi �Őݒ肳��Ă�����̂ł��BBSK ���g���Ă��Ȃ��ꍇ�́Awriteback �v���O�C���̓����̕ϐ��̒l�����̂܂܎g�p���ĉ������B

# writeback�̃f�[�^��ۑ�����f�B���N�g����
$writeback_dir = $blosxom::writeback_dir;

# writeback�̃f�[�^�t�@�C���̊g���q
$writeback_file_extension = $blosxom::writeback_file_extension;
�@�ǂ�����Awriteback �v���O�C���Őݒ肵�Ă���l�Ɠ������̂�ݒ肵�Ă��܂��B


��������
�E�\�����Ԃ��������Ă���̂ŁApaginate �Ȃǂ̃y�[�W����n�̃v���O�C���Ƃ͑����������ł��B
�@�ǂ����Ă��y�[�W���䂵�����ꍇ�́A$use_age �� 0 �ɐݒ肵�ĉ������B

�E�܂����܂�e�X�g���Ă܂���B
�@�����p�͎��ȐӔC�ŁI�i���s���[�h�j

�E�o�O�񍐂�v�]�Ȃǂ�����܂�����A���܂ŘA�����ĉ������B
�@���̌f���́Ahttp://cwww.pos.to/bbs/ �œ������Ă��܂��B

�E�Ĕz�z����ς͂����R�ɂǂ����B
�@newentry�v���O�C���ƃh�L�������g�̒��쌠�͎��i�[��@���j�ɂ���܂��B


���ӎ�
�@���̃v���O�C�������ɂ�����A�ȉ��̃��W���[����v���O�C�����Q�l�ɂ����Ē����܂����B

blosxom 2.0 http://www.blosxom.com/
Blosxom Starter Kit http://hail2u.net/archives/bsk.html (hai2u.net / kyo ����)
writeback �v���O�C�� http://www.blosxom.com/plugins/input/writeback.htm


������
2004/04/29 ���ō쐬
2005/05/28 �@�\����ō쐬
2005/08/20 XSS�Ǝ㐫�Ή��iandi��������L����A���w�E���肪�Ƃ��������܂����j

