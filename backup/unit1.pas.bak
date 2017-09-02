unit Unit1;

{$mode objfpc}{$H+}

interface

uses
  Classes, SysUtils, sqldb, IBConnection, FileUtil, SynEdit, Forms, Controls,
  Graphics, Dialogs, StdCtrls, ExtCtrls, ActnList, Menus;
type

  { TForm1 }

  TForm1 = class(TForm)
    Button1: TButton;
    Edit: TEdit;
    Edit1: TEdit;
    Edit10: TEdit;
    Edit11: TEdit;
    Edit12: TEdit;
    Edit13: TEdit;
    Edit14: TEdit;
    Edit15: TEdit;
    Edit16: TEdit;
    Edit17: TEdit;
    Edit18: TEdit;
    Edit19: TEdit;
    Edit2: TEdit;
    Edit20: TEdit;
    Edit21: TEdit;
    Edit22: TEdit;
    Edit23: TEdit;
    Edit24: TEdit;
    Edit25: TEdit;
    Edit26: TEdit;
    Edit27: TEdit;
    Edit28: TEdit;
    Edit29: TEdit;
    Edit3: TEdit;
    Edit30: TEdit;
    Edit35: TEdit;
    Edit36: TEdit;
    Edit37: TEdit;
    Edit38: TEdit;
    Edit39: TEdit;
    Edit4: TEdit;
    Edit40: TEdit;
    Edit41: TEdit;
    Edit42: TEdit;
    Edit43: TEdit;
    Edit45: TEdit;
    Edit5: TEdit;
    Edit50: TEdit;
    Edit6: TEdit;
    Edit7: TEdit;
    Edit8: TEdit;
    Edit9: TEdit;
    Label1: TLabel;
    Label10: TLabel;
    Label11: TLabel;
    Label12: TLabel;
    Label13: TLabel;
    Label14: TLabel;
    Label15: TLabel;
    Label16: TLabel;
    Label17: TLabel;
    Label18: TLabel;
    Label19: TLabel;
    Label2: TLabel;
    Label20: TLabel;
    Label21: TLabel;
    Label22: TLabel;
    Label23: TLabel;
    Label3: TLabel;
    Label4: TLabel;
    Label5: TLabel;
    Label6: TLabel;
    Label7: TLabel;
    Label8: TLabel;
    Label9: TLabel;
    procedure Button1Click(Sender: TObject);

    procedure EditChange(Sender: TObject);


  private
    { private declarations }
  public
    { public declarations }
  end;

var
  Form1: TForm1;
  pole, pole1, pole2, pole3, pole4, pole25, pole26, pole27, pole28, pole29, pole30, pole35, pole40: real;
  pole5, pole6, pole7, pole8, pole9, pole10, pole11, pole12, pole13, pole14, pole15: real;
  pole16, pole17, pole18, pole19, pole20, pole21, pole22, pole23, pole24: real;
   pole36, pole37, pole38, pole39,pole42,pole45, pole50,pole43, pole41  : real;
   zmienna: string;
   zmienna1: real;

implementation

{$R *.lfm}

{ TForm1 }

procedure TForm1.EditChange(Sender: TObject);
begin


end;




procedure TForm1.Button1Click(Sender: TObject);
begin


  pole:=StrToFloat(edit.text);
  pole1:=StrToFloat(edit1.text);
  pole2:=pole-pole1;
  pole3:=0;
  if pole2<0 then
   begin
  pole3:=abs(pole2);
  pole2:=0;
  end;

  pole4:=StrToFloat(edit4.text);

  pole5:=StrToFloat(edit5.text);
  pole6:=StrToFloat(edit6.text);

  pole8:=StrToFloat(edit8.text);
  pole9:=StrToFloat(edit9.text);

  pole10:=StrToFloat(edit10.text);
  pole11:=StrToFloat(edit11.text);

  pole13:=StrToFloat(edit13.text);
  pole14:=StrToFloat(edit14.text);

  pole15:=StrToFloat(edit15.text);
  pole16:=StrToFloat(edit16.text);

  pole18:=StrToFloat(edit18.text);
  pole19:=StrToFloat(edit19.text);

  pole20:=StrToFloat(edit20.text);
  pole21:=StrToFloat(edit21.text);

  pole23:=StrToFloat(edit23.text);
  pole24:=StrToFloat(edit24.text);




 pole25:=pole+pole5+pole10+pole15+pole20;
 pole26:=pole1+pole6+pole11+pole16+pole21;
  //suma dochodu
 pole28:=pole3+pole8+pole13+pole18+pole23;
 pole29:=pole4+pole9+pole14+pole19+pole24;
 pole30:=StrToFloat(edit30.text);


 edit2.text:=FloatToStr(pole2);
  edit3.text:=FloatToStr(pole3);
 edit7.text:= FloatToStr(pole5-pole6);
edit12.text:= FloatToStr(pole10-pole11);
edit17.text:= FloatToStr(pole15-pole16);
edit22.text:= FloatToStr(pole20-pole21);

 edit25.text:=FloatToStr(pole25);
 edit26.text:=FloatToStr(pole26);

 edit28.text:=FloatToStr(pole28);
 edit29.text:=FloatToStr(pole29);



 pole7:=StrToFloat(edit7.text);
 pole12:=StrToFloat(edit12.text);
 pole17:=StrToFloat(edit17.text);
 pole22:=StrToFloat(edit22.text);
 pole27:=pole2+pole7+pole12+pole17+pole22;

 edit27.text:=FloatToStr(pole27);

 pole36:=StrToFloat(edit35.text);


   pole35:=pole27-pole30;
  edit35.text:=FloatToStr(pole35);
  edit36.text:=edit35.text;

  pole38:=StrToFloat(edit36.text);
 edit38.text:=FormatFloat('0',pole38);
 pole38:=StrToFloat(edit38.text);

 pole39:=(pole38*0.18)-556.02;
 if pole39<0 then pole39:=0;
  pole37:=StrToFloat(edit37.text);//skladki na ubezpiecznia zdrowotne
  if pole41<pole37 then pole37:=pole41;
  edit37.text:=FormatFloat('0.00',pole37);
  pole42:=pole39-pole37;


 edit39.text:=FormatFloat('0.00',pole39);
 edit40.text:=FormatFloat('0',pole42);

 pole40:=StrToFloat(edit40.text);
 edit41.text:=edit39.text;//podatek
 pole41:=StrToFloat(edit41.text);
 edit42.text:=FormatFloat('0.00',pole42);
 edit45.text:=edit29.text;
 pole45:=StrToFloat(edit45.text);
 pole50:=pole40-pole45;   //Do zaplaty
  pole43:=0;  //Nadplata


  if pole50<0   then
   begin
     pole43:=Abs(pole50);
     pole50:=0;

   end;
 edit50.text:=FormatFloat('0',pole50);
 edit43.text:=FormatFloat('0',pole43);



   if pole50<=0 then
  showmessage ('Nadpłata: '+ edit43.text+' zł')
   else showmessage ('Do zapłaty: '+edit50.text+' zł.');
 end;

end.

