Windows��EGGX
Version 1.0
2014�N10��16��
���J �۔�
�i���d�C�ʐM��w�j


���͂��߂�

����́CWindows�p��C�iC++)����p��2�����O���t�B�b�N�X���C�u�����ł��D�L
���g���Ă���X11�O���t�B�b�N�X���C�u�����uEGGX/ProCALL�v

  http://www.ir.isas.jaxa.jp/~cyamauch/eggx_procall/index.ja.html

�̎d�l�i�̈ꕔ�j�ƌ݊��ɂȂ�悤�ɍ���Ă��܂��DEGGX/ProCALL�̍�҂�
����R�����iJAXA�j����uWindows��EGGX�v�Ɩ���邱�Ƃ̋��𓾂Ă��܂��D

���̃��C�u�����̓����́CEGGX�݊��ł��邱�ƂƁCWinAPI��S���ӎ����邱��
�Ȃ��Cmain()�֐��Ŏn�܂�C��C++�̃v���O�����Ŏg�����Ƃ��ł��邱�Ƃł��D


���g����

Visual Studio�̏ꍇ�C�v���W�F�N�g�̃v���p�e�B��3�����ɐݒ肪�K�v�ł��D

�EC/C++�́u�ǉ��̃C���N���[�h�f�B���N�g���v��
  �u�iwineggx�̃f�B���N�g���j\include�v��ǉ����Ă��������D

�E�����J�\�́u�ǉ��̃��C�u�����f�B���N�g���v��
  �u�iwineggx�̃f�B���N�g���j\lib�v��ǉ����Ă��������D

�E�����J�\�̓��͂́u�ǉ��̈ˑ��t�@�C���v�Ɂuwineggx.lib�v��ǉ����Ă��������D


���v���O�����̍���

�v���O�����̍ŏ��Ɂu#include <wineggx.h>�v��ǉ����Ă��������D�֐��̎g
�����́CEGGX��C�łƑS�������ł��D


���I���W�i���Ƃ̈Ⴂ

�u#include <eggx.h>�v�Ƃ������Ɂu#include <wineggx.h>�v�Ƃ��Ă��������D

�u#include <eggxlib.h>�v���g���ueggx_�v�Ŏn�܂�֐��ɂ͑Ή����Ă��܂���D

��������Ă���͈̂ȉ��̊֐������ł��D

------------------------------------------------------------------------
int gopen(int xsize,int ysize);
void gclose( int wn );
void gcloseall( void );
int winname( int wn, const char *argsformat, ... );
void window( int wn, double xs, double ys, double xe, double ye );
void layer( int wn, int lys, int lyw );
void copylayer( int wn, int lysrc, int lydest );
void newcolor( int wn, const char *argsformat, ... );
void newrgbcolor( int wn, int r, int g, int b );
void newhsvcolor( int wn, int h, int s, int v );
void gsetbgcolor( int wn, const char *argsformat, ... );
void gsetbgcolorrgb( int wn, int r, int g, int b );
void gclr( int wn );
void newlinewidth( int wn, int width );
void newlinestyle( int wn, int style );
void pset( int wn,double x,double y );
void drawline( int wn, double x0, double y0, double x1, double y1 );
void moveto( int wn, double x, double y );
void lineto( int wn, double x, double y );
void line( int wn,double x,double y,int mode );
void circle( int wn, double xcen, double ycen, double xrad, double yrad );
void fillcirc( int wn, double xcen, double ycen, double xrad, double yrad );
void drawarc( int wn, double xcen, double ycen, double xrad, double yrad, double sang, double eang, int idir );
void fillarc( int wn, double xcen, double ycen, double xrad, double yrad, double sang, double eang, int idir );
void drawrect( int wn, double x, double y, double w, double h );
void fillrect( int wn, double x, double y, double w, double h );
int drawstr( int wn, double x, double y, int size, double theta,const char *argsformat, ... );
int gsetfontset( int wn, const char *argsformat, ... );
int ggetch();
void gsetnonblock( int flag );
void msleep( unsigned long msec );
------------------------------------------------------------------------

�ȏ�D
