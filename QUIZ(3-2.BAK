#include<fstream.h>
#include<conio.h>
#include<stdio.h>
#include<process.h>
#include<string.h>
#include<ctype.h>
#include<dos.h>
#include<bios.h>
#include<graphics.h>
#include<stdlib.h>
//graphic functions
void loading()
{
 clrscr();
   /* request auto detection */
   int gdriver = DETECT, gmode, errorcode,n;
   char ch;
   /* initialize graphics mode */
   initgraph(&gdriver, &gmode, "C:\\TurboC3\\BGI");

   /* read result of initialization */
   errorcode = graphresult();

   if (errorcode != grOk)  /* an error occurred */
   {
      printf("Graphics error: %s\n", grapherrormsg(errorcode));
      printf("Press any key to halt:");
      getch();
      exit(1);             /* return with error code */
   }
settextstyle(SANS_SERIF_FONT,HORIZ_DIR,4);
  outtextxy(120,100,"LOADING");
  setbkcolor(BROWN);
   setcolor(WHITE);
   rectangle(170,175,500,200);
   setfillstyle(1,6);
   floodfill(190,190,WHITE);
settextstyle(SANS_SERIF_FONT,HORIZ_DIR,4);
   for(int i=0;170+2*i<485;i++)
   {
   outtextxy(170+2*i,166,"Û");
   delay(30);
   }
settextstyle(SANS_SERIF_FONT,HORIZ_DIR,2);
outtextxy(120,300,"Press Any key to continue");
getch();
closegraph();
}

void credits()
{
 clrscr();
   /* request auto detection */
   int gdriver = DETECT, gmode, errorcode,n;
   char ch;
   /* initialize graphics mode */
   initgraph(&gdriver, &gmode, "C:\\TurboC3\\BGI");

   /* read result of initialization */
   errorcode = graphresult();

   if (errorcode != grOk)  /* an error occurred */
   {
      printf("Graphics error: %s\n", grapherrormsg(errorcode));
      printf("Press any key to halt:");
      getch();
      exit(1);             /* return with error code */
   }


   setbkcolor(BROWN);
   setcolor(WHITE);

 for(int i=getmaxy();i>-200;i--)
 {
 cleardevice();
  settextstyle(SANS_SERIF_FONT,HORIZ_DIR,4);
  outtextxy(250,i,"CREDITS:");
  settextstyle(SANS_SERIF_FONT,HORIZ_DIR,3);
  outtextxy(120,i+40,"DONE BY");
  settextstyle(SANS_SERIF_FONT,HORIZ_DIR,2);
  outtextxy(120,i+70,"Rishav Roy");
  outtextxy(120,i+90,"Manish Shetty");
  outtextxy(120,i+110,"N.N.S. Subhash");
  settextstyle(SANS_SERIF_FONT,HORIZ_DIR,3);
  outtextxy(120,i+130,"SINCERE THANKS TO");
  settextstyle(SANS_SERIF_FONT,HORIZ_DIR,2);
  outtextxy(150,i+150,"Computer Science teacher:");
  outtextxy(120,i+170,"Uma Ma'am");
  delay(25);
   }
settextstyle(SANS_SERIF_FONT,HORIZ_DIR,2);
outtextxy(120,300,"Press Any key to Exit");
getch();
 closegraph();
}



void welcome()
{
  clrscr();
   /* request auto detection */
   int gdriver = DETECT, gmode, errorcode,n;
   char ch;
   /* initialize graphics mode */
   initgraph(&gdriver, &gmode, "C:\\TurboC3\\BGI");

   /* read result of initialization */
   errorcode = graphresult();

   if (errorcode != grOk)  /* an error occurred */
   {
      printf("Graphics error: %s\n", grapherrormsg(errorcode));
      printf("Press any key to halt:");
      getch();
      exit(1);             /* return with error code */
   }
int x,y,i;
	x=getmaxx()/2;
	y=getmaxy()/2;
	for(i=30;i<200;i++)
	{
		delay(10);
		setcolor(i/10);
		arc(x,y,0,180,i-10);
	}
settextstyle(SANS_SERIF_FONT,HORIZ_DIR,4);
outtextxy(120,300,"Welcome to the Quiz Show");
getch();
closegraph();
}

int password(void)
{
    qwerty: clrscr();
   /* request auto detection */
   int gdriver = DETECT, gmode, errorcode,n;
   char ch;
   /* initialize graphics mode */
   initgraph(&gdriver, &gmode, "C:\\TurboC3\\BGI");

   /* read result of initialization */
   errorcode = graphresult();

   if (errorcode != grOk)  /* an error occurred */
   {
      printf("Graphics error: %s\n", grapherrormsg(errorcode));
      printf("Press any key to halt:");
      getch();
      exit(1);             /* return with error code */
   }
   setbkcolor(GREEN);
   setcolor(WHITE);
   rectangle(170,170,500,250);
   setfillstyle(1,6);
   floodfill(190,190,WHITE);

   char password[50];
	int z=0;
	outtextxy(250,180," Enter the password");

	while(1){
	password[z]=getch();
		if(password[z]==8)
		{
			if(z<=0)
				z=0;
			else
			{
			--z;
			password[z]='\0';
			outtextxy(300+(10*z),200," ");
			}
		}
		else if(password[z]==13)
			break;
		else
		{
			outtextxy(300+(10*z),200,"*");
			z++;
		}
	}
	password[z]='\0';
	if(strcmp(password,"admin")!=0)
	{
		outtextxy(260,230,"Invalid password");
		getch();
		goto qwerty;

	}
	else
	 {
	     outtextxy(260,230,"Correct password");
	 }
   getch();
   closegraph();

   return 0;
}






//sturcture for player details
struct player
 {
   char fname[20],lname[20];
   int score;
 };

class sports
 {
   private:
       char q[200],a[50],b[50],c[50],d[50];
       char c_ans;
   public:
       void input()
	    { gotoxy(1,1);
	      cprintf("Question:");
	      gotoxy(1,2);
	      gets(q);
	      gotoxy(1,6);
	      cprintf("Options:");
	      gotoxy(1,8);
	      gets(a);
	      gets(b);
	      gets(c);
	      gets(d);
	      gotoxy(1,12);
	      cprintf("Correct answer");
	      gotoxy(1,13);
	      cin>>c_ans;
	    }
       void disp_q()
	    {
	      gotoxy(1,3);
	      cprintf("%s",q);
	      gotoxy(1,7);
	      cprintf("a.%s",a);
	      gotoxy(1,8);
	      cprintf("b.%s",b);
	      gotoxy(1,9);
	      cprintf("c.%s",c);
	      gotoxy(1,10);
	      cprintf("d.%s",d);

	    }
       char get_ans()
	    {
	    return(c_ans);
	    }
     };

  void sports_q_create()
    {textcolor(WHITE);
textbackground(BROWN);
clrscr();
    fstream x("sports.dat",ios::out|ios::binary);
    sports s;
    char ch;
    while(1)
    {
     s.input();
     x.write((char*)&s,sizeof(s));
     gotoxy(1,18);
     cprintf("Continue? Press n to exit");
     gotoxy(1,20);
     cin>>ch;
     if(ch=='N'||ch=='n')
      {break;}
     clrscr();
    }
    x.close();
    getch();
    }

    void sports_q_add()
    {textcolor(WHITE);
textbackground(BROWN);
clrscr();
    char ans ='Y';
    fstream x("sports.dat",ios::app|ios::binary);
    sports s1;
    while(ans=='y'||ans=='Y')
    {
    gotoxy(1,1);
	cprintf("Enter the question");
	gotoxy(1,2);
	s1.input();
	x.write((char*)&s1,sizeof(s1));
	gotoxy(1,20);
	cprintf("Continue? y/n");
    gotoxy(1,21);
    cin>>ans;
    clrscr();
    }
	x.close();
    }

    void sports_q_dispfile()
    {
    textcolor(WHITE);
textbackground(BROWN);
clrscr();
    fstream x("sports.dat",ios::in|ios::binary);
    sports s;
    int i=1;
    while(x.read((char*)&s,sizeof(s)))
    {
     clrscr();
	gotoxy(1,1);
	cprintf("Q.%d.",i);
	s.disp_q();
	gotoxy(1,18);
	cprintf("Correct Answer:  %c",s.get_ans());
	i++;
	getch();
    }
    x.close();
    }
    void sports_q_modify()
     {
     textcolor(WHITE);
textbackground(BROWN);
clrscr();
      char ans ='Y';
    fstream x("sports.dat",ios::in|ios::out|ios::binary);
    sports s;
    int qno;
    while(ans=='y'||ans=='Y')
    {
	gotoxy(1,1);
	cprintf("Enter the question no. to be modified: ");
	cin>>qno;
	getch();
	clrscr();
	x.seekg((qno-1)*sizeof(s),ios::beg);
	gotoxy(1,3);
	s.input();
	x.write((char*)&s,sizeof(s));
	gotoxy(1,20);
	cprintf("Continue? y/n");
	gotoxy(1,21);
	cin>>ans;
	clrscr();
    }
	x.close();

     }

    void play_sports(int n,player p[])
  {
    textcolor(WHITE);
textbackground(BROWN);
clrscr();


   char your_ans[5];
   fstream x("sports.dat",ios::in|ios::binary);
   sports s;
   //int q=10;
 //  randomize();
   for(int i=0;i<10;i++)
   {
     clrscr();

     //  x.seekg(random(q)*sizeof(s),ios::beg);
     x.read((char*)&s,sizeof(s));
     cprintf("Q%d.",i+1);
     s.disp_q();
      gotoxy(1,14);
     cprintf("Enter Response");
     for(int j=0;j<n;j++)
     {
	gotoxy(1,15+2*j);
	cprintf("%s %s :    ",p[j].fname,p[j].lname);
	cin>>your_ans[j];
       while(1)
       {
       if(your_ans[j]=='a'||your_ans[j]=='b'||your_ans[j]=='c'||your_ans[j]=='d')
	  break;
       else
	{
	    cprintf("Invalid answer!!! Enter correct answer");
	    cin>>your_ans[j];
	}
       }
       if(your_ans[j]==s.get_ans())
	 p[j].score+=3;
       else
	 p[j].score+=0;
     }
     getch();
     clrscr();
     gotoxy(1,5);
     cprintf("Correct Answer:  (%c)",s.get_ans());
      getch();
   }


  getch();
  }



  class entertainment
 {
   private:
       char q[200],a[50],b[50],c[50],d[50];
       char c_ans;
   public:
       void input()
	    { gotoxy(1,1);
	      cprintf("Question:");
	      gotoxy(1,2);
	      gets(q);
	      gotoxy(1,6);
	      cprintf("Options:");
	      gotoxy(1,8);
	      gets(a);
	      gets(b);
	      gets(c);
	      gets(d);
	      gotoxy(1,12);
	      cprintf("Correct answer");
	      gotoxy(1,13);
	      cin>>c_ans;
	    }
       void disp_q()
	    {
	      gotoxy(1,3);
	      cprintf("%s",q);
	      gotoxy(1,7);
	      cprintf("a.%s",a);
	      gotoxy(1,8);
	      cprintf("b.%s",b);
	      gotoxy(1,9);
	      cprintf("c.%s",c);
	      gotoxy(1,10);
	      cprintf("d.%s",d);

	    }
       char get_ans()
	    {
	    return(c_ans);
	    }
     };

  void entertainment_q_create()
    {
	textcolor(WHITE);
textbackground(BROWN);
clrscr();
    fstream x("entertainment.dat",ios::out|ios::binary);
    entertainment e ;
    char ch;
    while(1)
    {
     e.input();
     x.write((char*)&e,sizeof(e));
      gotoxy(1,18);
     cprintf("Continue? Press n to exit");
     gotoxy(1,20);
     cin>>ch;
     if(ch=='N'||ch=='n')
      {break;}
     clrscr();
    }
    x.close();
    getch();
    }

    void entertainment_q_add()
    {
	textcolor(WHITE);
textbackground(BROWN);
clrscr();
    char ans ='Y';
    fstream x("entertainment.dat",ios::app|ios::binary);
    entertainment e1;
    while(ans=='y'||ans=='Y')
    {
	gotoxy(1,1);
	cprintf("Enter the question");
	gotoxy(1,2);
	e1.input();
	x.write((char*)&e1,sizeof(e1));
	gotoxy(1,20);
	cprintf("Continue? y/n");
    gotoxy(1,21);
    cin>>ans;
    clrscr();
    }
	x.close();
    }

void entertainment_q_dispfile()
    {

textcolor(WHITE);
textbackground(BROWN);
clrscr();
    fstream x("entertainment.dat",ios::in|ios::binary);
    entertainment e;
    int i=1;
    while(x.read((char*)&e,sizeof(e)))
    {
	clrscr();
	gotoxy(1,1);
	cprintf("Q%d.",i);
	e.disp_q();
	gotoxy(1,18);
	cprintf("Correct Answer:  %c",e.get_ans());
	getch();
	i++;
    }
    x.close();
    }
 void entertainment_q_modify()
     {
     textcolor(WHITE);
textbackground(BROWN);
clrscr();
      char ans ='Y';
    fstream x("entertainment.dat",ios::in|ios::out|ios::binary);
    entertainment e;
    int qno;
    while(ans=='y'||ans=='Y')
    {
	gotoxy(1,1);
	cprintf("Enter the question no. to be modified: ");
	cin>>qno;
	getch();
	clrscr();
	x.seekg((qno-1)*sizeof(e),ios::beg);
	gotoxy(1,3);
	e.input();
	x.write((char*)&e,sizeof(e));
	gotoxy(1,20);
	cprintf("Continue? y/n");
	gotoxy(1,21);
	cin>>ans;
	clrscr();
    }
	x.close();

     }

    void play_entertainment(int n,player p[])
  {textcolor(WHITE);
textbackground(BROWN);

    clrscr();
   //int q=10;
   char your_ans[5];
   fstream x("entertainment.dat",ios::in|ios::binary);
   entertainment e ;
   for(int i=0;i<10;i++)
   {
     clrscr();
   //  randomize();
   //  x.seekg(random(q)*sizeof(e),ios::beg);
     x.read((char*)&e,sizeof(e));
     cprintf("Q%d.",i+1);
     e.disp_q();
       gotoxy(1,14);
     cprintf("Enter Response");
     for(int j=0;j<n;j++)
     {
	gotoxy(1,15+2*j);
	cprintf("%s %s :    ",p[j].fname,p[j].lname);
	cin>>your_ans[j];
       while(1)
       {
       if(your_ans[j]=='a'||your_ans[j]=='b'||your_ans[j]=='c'||your_ans[j]=='d')
	  break;
       else
	{
	    cprintf("Invalid answer!!! Enter correct answer");
	    cin>>your_ans[j];
	}
       }
       if(your_ans[j]==e.get_ans())
	 p[j].score+=3;
       else
	 p[j].score+=0;
     }
     getch();
     clrscr();

     gotoxy(1,5);
     cprintf("Correct Answer:  (%c)",e.get_ans());
      getch();
   }
  getch();
  }


 class food
 {
   private:
       char q[200],a[50],b[50],c[50],d[50];
       char c_ans;
   public:
      void input()
	    { gotoxy(1,1);
	      cprintf("Question:");
	      gotoxy(1,2);
	      gets(q);
	      gotoxy(1,6);
	      cprintf("Options:");
	      gotoxy(1,8);
	      gets(a);
	      gets(b);
	      gets(c);
	      gets(d);
	      gotoxy(1,12);
	      cprintf("Correct answer");
	      gotoxy(1,13);
	      cin>>c_ans;
	    }
       void disp_q()
	    {
	      gotoxy(1,3);
	      cprintf("%s",q);
	      gotoxy(1,7);
	      cprintf("a.%s",a);
	      gotoxy(1,8);
	      cprintf("b.%s",b);
	      gotoxy(1,9);
	      cprintf("c.%s",c);
	      gotoxy(1,10);
	      cprintf("d.%s",d);

	    }
       char get_ans()
	    {
	    return(c_ans);
	    }
     };

  void food_q_create()
    {
	textcolor(WHITE);
textbackground(BROWN);
clrscr();
    fstream x("food.dat",ios::out|ios::binary);
    food f ;
    char ch;
    while(1)
    {
     f.input();
     x.write((char*)&f,sizeof(f));
     gotoxy(1,18);
     cprintf("Continue? Press n to exit");
     gotoxy(1,20);
     cin>>ch;
     if(ch=='N'||ch=='n')
      {break;}
     clrscr();
    }

    x.close();
    getch();
    }

    void food_q_add()
    {
	textcolor(WHITE);
textbackground(BROWN);
clrscr();
     char ans ='Y';
    fstream x("food.dat",ios::app|ios::binary);
    food f1;
    while(ans=='y'||ans=='Y')
    {
	gotoxy(1,1);
	cprintf("Enter the question");
	gotoxy(1,2);
	f1.input();
	x.write((char*)&f1,sizeof(f1));
	gotoxy(1,20);
	cprintf("Continue? y/n");
    gotoxy(1,21);
    cin>>ans;
    clrscr();
    }
	x.close();
    }

void food_q_dispfile()
    {
    textcolor(WHITE);
textbackground(BROWN);
clrscr();
    fstream x("food.dat",ios::in|ios::binary);
    food f;
    int i=1;
    while(x.read((char*)&f,sizeof(f)))
    {
	clrscr();
	gotoxy(1,1);
	cprintf("Q%d.",i);
	f.disp_q();
	gotoxy(1,18);
	cprintf("%c",f.get_ans());
	getch();
	i++;
    }
    x.close();
    }

   void food_q_modify()
     {
     textcolor(WHITE);
textbackground(BROWN);
clrscr();
      char ans ='Y';
    fstream x("food.dat",ios::in|ios::out|ios::binary);
    food f;
    int qno;
    while(ans=='y'||ans=='Y')
    {
	gotoxy(1,1);
	cprintf("Enter the question no. to be modified: ");
	cin>>qno;
	getch();
	clrscr();
	x.seekg((qno-1)*sizeof(f),ios::beg);
	gotoxy(1,3);
	f.input();
	x.write((char*)&f,sizeof(f));
	gotoxy(1,20);
	cprintf("Continue? y/n");
	gotoxy(1,21);
	cin>>ans;
	clrscr();
    }
	x.close();

     }

    void play_food(int n,player p[])
  {
    textcolor(WHITE);
textbackground(BROWN);
clrscr();
//   int q=10;
   char your_ans[5];
   fstream x("food.dat",ios::in|ios::binary);
   food f;
   for(int i=0;i<10;i++)
   {
     clrscr();
    // randomize();

//     x.seekg(random(q)*sizeof(f),ios::beg);
     x.read((char*)&f,sizeof(f));
     cprintf("Q%d.",i+1);
     f.disp_q();
      gotoxy(1,14);
     cprintf("Enter Response");
     for(int j=0;j<n;j++)
     {
	gotoxy(1,15+2*j);
	cprintf("%s %s :    ",p[j].fname,p[j].lname);
	cin>>your_ans[j];
       while(1)
       {
       if(your_ans[j]=='a'||your_ans[j]=='b'||your_ans[j]=='c'||your_ans[j]=='d')
	  break;
       else
	{
	    cprintf("Invalid answer!!! Enter correct answer");
	    cin>>your_ans[j];
	}
       }
       if(your_ans[j]==f.get_ans())
	 p[j].score+=3;
       else
	 p[j].score+=0;
     }
     getch();
     clrscr();
     gotoxy(1,5);
     cprintf("Correct Answer:  (%c)",f.get_ans());
      getch();
       }
  getch();
  }

  class GK
 {
   private:
       char q[200],a[50],b[50],c[50],d[50];
       char c_ans;
   public:
      void input()
	    { gotoxy(1,1);
	      cprintf("Question:");
	      gotoxy(1,2);
	      gets(q);
	      gotoxy(1,6);
	      cprintf("Options:");
	      gotoxy(1,8);
	      gets(a);
	      gets(b);
	      gets(c);
	      gets(d);
	      gotoxy(1,12);
	      cprintf("Correct answer");
	      gotoxy(1,13);
	      cin>>c_ans;
	    }
       void disp_q()
	    {
	      gotoxy(1,3);
	      cprintf("%s",q);
	      gotoxy(1,7);
	      cprintf("a.%s",a);
	      gotoxy(1,8);
	      cprintf("b.%s",b);
	      gotoxy(1,9);
	      cprintf("c.%s",c);
	      gotoxy(1,10);
	      cprintf("d.%s",d);

	    }
       char get_ans()
	    {
	    return(c_ans);
	    }
     };

  void GK_q_create()
    {
	textcolor(WHITE);
textbackground(BROWN);
clrscr();
    fstream x("GK.dat",ios::out|ios::binary);
    GK g;
    char ch;
    while(1)
    {
     g.input();
     x.write((char*)&g,sizeof(g));
      gotoxy(1,18);
     cprintf("Continue? Press n to exit");
     gotoxy(1,20);
     cin>>ch;
     if(ch=='N'||ch=='n')
      {break;}
     clrscr();
    }
    x.close();
    getch();
    }

    void GK_q_add()
    {

     textcolor(WHITE);
textbackground(BROWN);
clrscr();
char ans ='Y';
    fstream x("GK.dat",ios::app|ios::binary);
    GK g1;
    while(ans=='y'||ans=='Y')
    {
	gotoxy(1,1);
	cprintf("Enter the question");
	gotoxy(1,2);
	g1.input();
	x.write((char*)&g1,sizeof(g1));
	gotoxy(1,20);
	cprintf("Continue? y/n");
    gotoxy(1,21);
    cin>>ans;
    clrscr();
    }
	x.close();
	}

void GK_q_dispfile()
    {
    textcolor(WHITE);
textbackground(BROWN);
clrscr();
    fstream x("GK.dat",ios::in|ios::binary);
    GK g;
    int i=1;
    while(x.read((char*)&g,sizeof(g)))
    {
	clrscr();
	gotoxy(1,1);
	cprintf("Q%d.",i);
	g.disp_q();
	gotoxy(1,18);
	cprintf("%c",g.get_ans());
	getch();
	i++;
    }
    x.close();
    }
 void GK_q_modify()
     {
     textcolor(WHITE);
textbackground(BROWN);
clrscr();
      char ans ='Y';
    fstream x("GK.dat",ios::in|ios::out|ios::binary);
    GK g;
    int qno;
    while(ans=='y'||ans=='Y')
    {
	gotoxy(1,1);
	cprintf("Enter the question no. to be modified: ");
	cin>>qno;
	getch();
	clrscr();
	x.seekg((qno-1)*sizeof(g),ios::beg);
	gotoxy(1,3);
	g.input();
	x.write((char*)&g,sizeof(g));
	gotoxy(1,20);
	cprintf("Continue? y/n");
	gotoxy(1,21);
	cin>>ans;
	clrscr();
    }
	x.close();

     }

    void play_GK(int n,player p[])
  {
    textcolor(WHITE);
textbackground(BROWN);
clrscr();
  // int q=10;
   char your_ans[5];
   fstream x("GK.dat",ios::in|ios::binary);
   GK g;
   for(int i=0;i<10;i++)
   {
      clrscr();
    // randomize();

    // x.seekg(random(q)*sizeof(g),ios::beg);

     x.read((char*)&g,sizeof(g));
     cprintf("Q%d.",i+1);
     g.disp_q();
      gotoxy(1,14);
     cprintf("Enter Response");
     for(int j=0;j<n;j++)
     {
	gotoxy(1,15+2*j);
	cprintf("%s %s :    ",p[j].fname,p[j].lname);
	cin>>your_ans[j];
       while(1)
       {
       if(your_ans[j]=='a'||your_ans[j]=='b'||your_ans[j]=='c'||your_ans[j]=='d')
	  break;
       else
	{
	    cprintf("Invalid answer!!! Enter correct answer");
	    cin>>your_ans[j];
	}
       }
       if(your_ans[j]==g.get_ans())
	 p[j].score+=3;
       else
	 p[j].score+=0;
     }
     getch();
     clrscr();

     gotoxy(1,5);
     cprintf("Correct Answer:  (%c)",g.get_ans());
      getch();
   }
  getch();
  }


  class Politics
 {
   private:
       char q[200],a[80],b[80],c[80],d[80];
       char c_ans;
   public:
      void input()
	    { gotoxy(1,1);
	      cprintf("Question:");
	      gotoxy(1,2);
	      gets(q);
	      gotoxy(1,6);
	      cprintf("Options:");
	      gotoxy(1,8);
	      gets(a);
	      gets(b);
	      gets(c);
	      gets(d);
	      gotoxy(1,12);
	      cprintf("Correct answer");
	      gotoxy(1,13);
	      cin>>c_ans;
	    }
       void disp_q()
	    {
	      gotoxy(1,3);
	      cprintf("%s",q);
	      gotoxy(1,7);
	      cprintf("a.%s",a);
	      gotoxy(1,8);
	      cprintf("b.%s",b);
	      gotoxy(1,9);
	      cprintf("c.%s",c);
	      gotoxy(1,10);
	      cprintf("d.%s",d);

	    }
       char get_ans()
	    {
	    return(c_ans);
	    }
     };

  void politics_q_create()
    {textcolor(WHITE);
textbackground(BROWN);
clrscr();
    fstream x("Politics.dat",ios::out|ios::binary);
    Politics pol;
    char ch;
    while(1)
    {
     pol.input();
     x.write((char*)&pol,sizeof(pol));
      gotoxy(1,18);
     cprintf("Continue? Press n to exit");
     gotoxy(1,20);
     cin>>ch;
     if(ch=='N'||ch=='n')
      {break;}
     clrscr();
    }
    x.close();
    getch();
    }

    void politics_q_add()
    {textcolor(WHITE);
textbackground(BROWN);
clrscr();
    char ans ='Y';
    fstream x("Politics.dat",ios::app|ios::binary);
    Politics pol1;
    while(ans=='y'||ans=='Y')
    {
	gotoxy(1,1);
	cprintf("Enter the question");
	gotoxy(1,2);
	pol1.input();
	x.write((char*)&pol1,sizeof(pol1));
	gotoxy(1,20);
	cprintf("Continue? y/n");
    gotoxy(1,21);
    cin>>ans;
    clrscr();
    }
	x.close();
    }

void politics_q_dispfile()
    {
    textcolor(WHITE);
textbackground(BROWN);
clrscr();
    fstream x("Politics.dat",ios::in|ios::binary);
    Politics pol;
    int i=1;
    while(x.read((char*)&pol,sizeof(pol)))
    {
	clrscr();
	gotoxy(1,1);
	cprintf("Q%d.",i);
	pol.disp_q();
	gotoxy(1,18);
	cprintf("%c",pol.get_ans());
	getch();
	i++;
    }
    x.close();
    }
    void politics_q_modify()
     {
     textcolor(WHITE);
textbackground(BROWN);
clrscr();
      char ans ='Y';
    fstream x("Politics.dat",ios::in|ios::out|ios::binary);
    Politics pol;
    int qno;
    while(ans=='y'||ans=='Y')
    {
	gotoxy(1,1);
	cprintf("Enter the question no. to be modified: ");
	cin>>qno;
	getch();
	clrscr();
	x.seekg((qno-1)*sizeof(pol),ios::beg);
	gotoxy(1,3);
	pol.input();
	x.write((char*)&pol,sizeof(pol));
	gotoxy(1,20);
	cprintf("Continue? y/n");
	gotoxy(1,21);
	cin>>ans;
	clrscr();
    }
	x.close();

     }

    void play_politics(int n,player p[])
  {
    textcolor(WHITE);
textbackground(BROWN);
clrscr();

   char your_ans[5];
   fstream x("Politics.dat",ios::in|ios::binary);
   Politics pol;
 //  int q=10;
   for(int i=0;i<10;i++)
   {
      clrscr();
   //  randomize();

   //  x.seekg(random(q)*sizeof(pol),ios::beg);
     cprintf("Q%d.",i+1);
     x.read((char*)&pol,sizeof(pol));
     pol.disp_q();
      gotoxy(1,14);
     cprintf("Enter Response");
     for(int j=0;j<n;j++)
     {
	gotoxy(1,15+2*j);
	cprintf("%s %s :    ",p[j].fname,p[j].lname);
	cin>>your_ans[j];
       while(1)
       {
       if(your_ans[j]=='a'||your_ans[j]=='b'||your_ans[j]=='c'||your_ans[j]=='d')
	  break;
       else
	{
	    cprintf("Invalid answer!!! Enter correct answer");
	    cin>>your_ans[j];
	}
       }
       if(your_ans[j]==pol.get_ans())
	 p[j].score+=3;
       else
	 p[j].score+=0;
     }
     getch();
     clrscr();

     gotoxy(1,5);
     cprintf("Correct Answer:  (%c)",pol.get_ans());
      getch();
    }
  getch();
  }


  void print_score(int n,player p[])
  {
    textcolor(WHITE);
textbackground(BROWN);
clrscr();
    int i,j;
    player temp;
    for(i=0;i<n;i++)
    {
      for(j=i+1;j<n;j++)
      {
	  if(p[i].score<p[j].score)
	  {
	      temp=p[i];
	      p[i]=p[j];
	      p[j]=temp;
	  }
      }
    }
   gotoxy(35,4);
   cprintf("Scores");
   gotoxy(5,7);
   cprintf("Position       First Name        Last Name        Scores");
   gotoxy(5,8);
   cprintf("________________________________________________________");
   for(int k=0;k<n;k++)
   {
       int o=k+1;
   gotoxy(5,10+k*2);
   cprintf("%d",o);
   gotoxy(20,10+k*2);
   cprintf("%s",p[k].fname);
   gotoxy(38,10+k*2);
   cprintf("%s",p[k].lname);
   gotoxy(55,10+k*2);
   cprintf("%d",p[k].score);
   }
  }



  void accept_player(int n,player p[])
  {
      textcolor(WHITE);
textbackground(BROWN);
clrscr();
      for(int i=0;i<n;i++)
      {
	  int o=i+1;
	 gotoxy(26,10);//1,1+i*5
	 cprintf("Player %d",o);
	 gotoxy(30,12);//8,2+i*5
	 cprintf("First Name:  ");
	  scanf("%s",&p[i].fname);
	 gotoxy(30,13);//8,3+i*5
	 cprintf("Last Name:   ");
	  scanf("%s",&p[i].lname);
	  p[i].score=0;
	  clrscr();
      }
  }






class TieBreaker
 {
   private:
       char q[200],a[80],b[80],c[80],d[80];
       char c_ans;
   public:
       void input()
	    {
	      gotoxy(1,1);
	      cprintf("Question:");
	      gotoxy(1,2);
	      gets(q);
	      gotoxy(1,6);
	      cprintf("Options:");
	      gotoxy(1,8);
	      gets(a);
	      gets(b);
	      gets(c);
	      gets(d);
	      gotoxy(1,12);
	      cprintf("Correct answer");
	      gotoxy(1,13);
	      cin>>c_ans;
	    }
       void disp_q()
	    {
	      gotoxy(1,3);
	      cprintf("%s",q);
	      gotoxy(1,7);
	      cprintf("a.%s",a);
	      gotoxy(1,8);
	      cprintf("b.%s",b);
	      gotoxy(1,9);
	      cprintf("c.%s",c);
	      gotoxy(1,10);
	      cprintf("d.%s",d);

	    }
       char get_ans()
	    {
	    return(c_ans);
	    }
     };

  void TieBreaker_q_create()
    {
	textcolor(WHITE);
textbackground(BROWN);
clrscr();
    fstream x("TieBreaker.dat",ios::out|ios::binary);
    TieBreaker t;
    char ch;
    while(1)
    {
     t.input();
     x.write((char*)&t,sizeof(t));
     gotoxy(1,18);
     cprintf("Continue? Press n to exit");
     gotoxy(1,20);
     cin>>ch;
     if(ch=='N'||ch=='n')
      {break;}
     clrscr();
    }
    x.close();
    getch();
    }

    void TieBreaker_q_add()
    {
	textcolor(WHITE);
textbackground(BROWN);
clrscr();
    char ans ='Y';
    fstream x("TieBreaker.dat",ios::app|ios::binary);
    TieBreaker t1;
    while(ans=='y'||ans=='Y')
    {
	gotoxy(1,1);
	cprintf("Enter the question");
	gotoxy(1,2);
	t1.input();
	x.write((char*)&t1,sizeof(t1));
	gotoxy(1,20);
	cprintf("Continue? y/n");
    gotoxy(1,21);
    cin>>ans;
    clrscr();
    }
	x.close();
    }

void TieBreaker_q_dispfile()
    {
     textcolor(WHITE);
textbackground(BROWN);
clrscr();
    clrscr();
    fstream x("TieBreaker.dat",ios::in|ios::binary);
    TieBreaker t;
    int i=1;
    while(x.read((char*)&t,sizeof(t)))
    {
	 clrscr();
	gotoxy(1,1);
	cprintf("Q%d.",i);
	t.disp_q();
	gotoxy(1,18);
	cprintf("%c",t.get_ans());
	getch();
	i++;
    }
    x.close();
    getch();
    }

    void TieBreaker_q_modify()
     {
     textcolor(WHITE);
textbackground(BROWN);
clrscr();
      char ans ='Y';
    fstream x("TieBreaker.dat",ios::in|ios::out|ios::binary);
    TieBreaker t;
    int qno;
    while(ans=='y'||ans=='Y')
    {
	gotoxy(1,1);
	cprintf("Enter the question no. to be modified: ");
	cin>>qno;
	getch();
	clrscr();
	x.seekg((qno-1)*sizeof(t),ios::beg);
	gotoxy(1,3);
	t.input();
	x.write((char*)&t,sizeof(t));
	gotoxy(1,20);
	cprintf("Continue? y/n");
	gotoxy(1,21);
	cin>>ans;
	clrscr();
    }
	x.close();

     }
    void play_TieBreaker(int c,player p[])
  {
    textcolor(WHITE);
textbackground(BROWN);
clrscr();
   char your_ans[5];
   fstream x("TieBreaker.dat",ios::in|ios::binary);
   TieBreaker t;;
   //int q=10;
   for(int i=0;i<10;i++)
   {
      clrscr();
     //randomize();
     //x.seekg(random(q)*sizeof(pol),ios::beg);
     cprintf("Q%d.",i+1);
     x.read((char*)&t,sizeof(t));
     t.disp_q();
     gotoxy(1,14);
     cprintf("Enter Response");
     for(int j=0;j<c;j++)
     {
	gotoxy(1,15+2*j);
	cprintf("%s %s :    ",p[j].fname,p[j].lname);
	cin>>your_ans[j];
       while(1)
       {
       if(your_ans[j]=='a'||your_ans[j]=='b'||your_ans[j]=='c'||your_ans[j]=='d')
	  break;
       else
	{
	    cprintf("Invalid answer!!! Enter correct answer");
	    cin>>your_ans[j];
	}
       }
	if(your_ans[j]==t.get_ans())
	 p[j].score+=3;
       else
	 p[j].score+=0;
     }
     getch();
     clrscr();
     gotoxy(1,5);
     cprintf("Correct Answer:  (%c)",t.get_ans());
    }
  getch();
  }

void score_print(int n,player p[5])
{
    textcolor(WHITE);
textbackground(BROWN);
clrscr();
   gotoxy(35,10);
   textcolor( BLACK + BLINK);
   cprintf(p[0].fname);
   cprintf(" ");
   textcolor( WHITE + BLINK);
    cprintf(p[0].lname);
    textcolor( BLUE + BLINK);
    cprintf(" Wins");


    //RISHAV LOOK HERE
    for (int i = 1;i<n;i++)
	{
	if(p[i].score==p[0].score)
    {
   gotoxy(35,11+i);
   textcolor( WHITE + BLINK);
   cprintf(p[i].fname);
   cprintf(" ");
   textcolor( WHITE + BLINK);
    cprintf(p[i].lname);
    textcolor( BLUE + BLINK);
    cprintf(" Wins");

    }
    getch();
    textcolor(WHITE);
    textbackground(BROWN);
    clrscr();
    }
  }

char warning()
{
 char ch;
  textcolor(WHITE);
textbackground(BROWN);
clrscr();
gotoxy(10,10);
cprintf("Are you sure you want to create a new file...");
gotoxy(10,12);
cprintf("To create a new file the old file will be permanently deleted");
gotoxy(10,14);
cprintf("Continue y/n?");
cin>>ch;
return ch;
}


void disp(int n)
{
int i=1;
char menu[7][20]={"GAME MODES:","Sports","Entertainment","Food","GK","Politics","EXIT"};
textcolor(WHITE);
textbackground(BROWN);
clrscr();

	gotoxy(38,5);
	for(i=1;i<=7;i++)
	{
		if(i==n)
			{
			textbackground(BLACK);
			textcolor(RED);
			gotoxy(34,5+i*2);//+1
			cprintf("%s\n",menu[i-1]);
			textbackground(BROWN);
			textcolor(WHITE);
			}
		else{
		gotoxy(34,5+i*2);//+1
		textcolor(WHITE);
		cprintf("%s\n",menu[i-1]);
		}
	}
}

  void disp2(int m)
{
int i=1;
char menu[4][20]={"MENU :","---> ADMIN","---> PLAY GAME","---> EXIT"};

textcolor(WHITE);
textbackground(BROWN);
clrscr();
	gotoxy(38,7);//1,1
	for(i=1;i<=4;i++)
	{
		if(i==m)
			{
			textbackground(BLACK);
			textcolor(RED);
			gotoxy(34,7+i*2);//+1.........1,i
			cprintf("%s\n",menu[i-1]);
			textbackground(BROWN);
			textcolor(WHITE);
			}
		else{
		gotoxy(34,7+i*2);//+1.........1,i
		textcolor(WHITE);
		cprintf("%s\n",menu[i-1]);
		}
	}
}
 void disp3(int l)
{
int i=1;
char menu[6][30]={"CHOICE:","(*) Create a new quiz file","(*) Add new questions","(*) Display all questions","(*) Modify questions","(*) Go to main menu"};

textcolor(WHITE);
textbackground(BROWN);
clrscr();
	gotoxy(38,4);
	for(i=1;i<=6;i++)
	{
		if(i==l)
			{
			textbackground(BLACK);
			textcolor(RED);
			gotoxy(27,5+i*2);//+1
			cprintf("%s\n",menu[i-1]);
			textbackground(BROWN);
			textcolor(WHITE);
			}
		else{
		gotoxy(27,5+i*2);//+1
		textcolor(WHITE);
		cprintf("%s\n",menu[i-1]);
		}
	}
}
void disp4(int p)
{
int i=1;
char menu[8][20]={"TYPE:","Sports","Entertainment","Food","GK","Politics","Tie Breaker","EXIT"};

textcolor(WHITE);
textbackground(BROWN);
clrscr();
	gotoxy(38,5);
	for(i=1;i<=8;i++)
	{
		if(i==p)
			{
			textbackground(BLACK);
			textcolor(RED);
			gotoxy(34,5+i*2);//+1
			cprintf("%s\n",menu[i-1]);
			textbackground(BROWN);
			textcolor(WHITE);
			}
		else{
		gotoxy(34,5+i*2);//+1
		textcolor(WHITE);
		cprintf("%s\n",menu[i-1]);
		}
	}
}

  void main()
  {
    welcome();
   textcolor(WHITE);
   textbackground(BROWN);
   clrscr();
   char ch;

	       clrscr();
	       MAINMENU:
	       int c,M=2;
		    disp2(2);
		    gotoxy(1,M);

		    while((c=bioskey(0))!=75)
		    {
			gotoxy(1,M);
			if(c==20480){

			    if(M<=4)
			    {
				M=M+1;
				disp2(M);//i-1
				gotoxy(1,M);
			    }
			    else{}
				    }

			 else if(c==18432){
			if(M>2){
				M=M-1;
				disp2(M);//i-1
				gotoxy(1,M);
				}
					   }

			else if (c==7181)  //if enter is pressed in the main menu
			{

	if(M==2)     //admin is selected
		{
		  password();
		   //if password is correct it comes here

		  adminmenu:

		  int o,i=2;
		  disp3(2);
		  gotoxy(1,i);

		    while((o=bioskey(0))!=75)
		    {
			gotoxy(1,i);
			if(o==20480){

			    if(i<=6){

				i=i+1;
				disp3(i);//i-1
				gotoxy(1,i);
				    }
			    else{}

			}

			else if(o==18432){

			     if(i>2){

				i=i-1;
				disp3(i);//i-1
				gotoxy(1,i);
				    }
			}

			else if (o==7181){     //entered into admin

			     if(i==2){
			     flag2:
			     int p,i=2;
			     disp4(2);
			     gotoxy(1,i);

		    while((p=bioskey(0))!=75)
		    {
			gotoxy(1,i);
			if(p==20480){

			    if(i<=8){

				i=i+1;
				disp4(i);//i-1
				gotoxy(1,i);

				}
			    else{}
			}
		       else if(p==18432){

			    if(i>2){

				i=i-1;
				disp4(i);//i-1
				gotoxy(1,i);

				}
			}

		      else if (p==7181){

			   if(i==2)
		    {

			clrscr();
			if(warning()=='y')
			 sports_q_create();
			getch();
		    goto flag2;	//break;
		    }
			   else if (i==3)
		    {
			clrscr();
			if(warning()=='y')
			entertainment_q_create();
			getch();
		      goto flag2;	//break;
		    }
			   else if(i==4)
		    {
			clrscr();
			if(warning()=='y')
			food_q_create();
			getch();
			goto flag2;//break;
		    }
			   else if (i==5)
		    {
			clrscr();
			if(warning()=='y')
			GK_q_create();
			getch();
			goto flag2;//break;
		    }
			  else if (i==6)
		    {
			clrscr();
			if(warning()=='y')
			politics_q_create();
			getch();
			goto flag2;//break;
		    }
			  else if(i==7)
		    {	clrscr();
			if(warning()=='y')
			TieBreaker_q_create();
			getch();
			goto flag2;//break;
		    }

			else if(i==8)
		    {
		      goto adminmenu; //	cprintf("Enter correct choice");
		       //break;
		    }
		    }
		    }// while loop closed
		 getch();
		break;
		 }// create quiz file closed




	else if(i==3){        //add questions opened
		    flag3:
		    int h,i=2;
		    disp4(2);
		    gotoxy(1,i);

		    while((h=bioskey(0))!=75)
		    {
			gotoxy(1,i);
			if(h==20480){

			    if(i<=8){
				i=i+1;
				disp4(i);//i-1
				gotoxy(1,i);
				    }
			    else{}
				     }

			else if(h==18432){

			if(i>2){
				i=i-1;
				disp4(i);//i-1
				gotoxy(1,i);
				}
					  }

			else if (h==7181)
			{

			if(i==2)
		    {
			clrscr();
			sports_q_add();
			getch();
			goto flag3;//break;
		    }
			else if(i==3)
		    {
			clrscr();
			entertainment_q_add();
			getch();
			goto flag3;//break;
		    }
			else if(i==4)
		    {

			clrscr();
			food_q_add();
			getch();
			goto flag3;//break;
		    }
			else if(i==5)
		    {
			clrscr();
			GK_q_add();
			getch();
			goto flag3;//break;
		    }
			else if(i==6)
		    {
			clrscr();
			politics_q_add();
			getch();
			goto flag3;//break;
		    }
			else if(i==7)
		    {    clrscr();
			 TieBreaker_q_add();
			 getch();
			 goto flag3;//break;
		    }

			else if(i==8)
		    {
		       //	cprintf("Enter correct choice");
			goto adminmenu;//break;
		    }
		    }
		    } //while loop closed
		  getch();
		  //break;
		}//add questions closed


     else if (i==4)      //display questions opened
		{  flag4:
		    int j,i=2;
		    disp4(2);
		    gotoxy(1,i);

		    while((j=bioskey(0))!=75)
		    {
			gotoxy(1,i);
			if(j==20480){
			    if(i<=8){
				i=i+1;
				disp4(i);//i-1
				gotoxy(1,i);
			    }
			    else{}
			}
			 else if(j==18432){
			if(i>2){
				i=i-1;
				disp4(i);//i-1
				gotoxy(1,i);
			}
			}

			 else if (j==7181){

			if(i==2)
		       {
			clrscr();
			sports_q_dispfile();
			getch();
		      goto flag4 ; //	break;
		    }
			else if(i==3)
		    {
			clrscr();
			entertainment_q_dispfile();
			getch();
		       goto flag4; //	break;
		    }
			else if(i==4)
		    {

			clrscr();
			food_q_dispfile();
			getch();
		       goto flag4; //	break;
		    }
			else if (i==5)
		    {
			clrscr();
			GK_q_dispfile();
			getch();
		      goto flag4; //	break;
		    }
			else if (i==6)
		    {
			clrscr();
			politics_q_dispfile();
			getch();
			goto flag4;//break;
		    }
			else if(i==7)
		    {   clrscr();
			TieBreaker_q_dispfile();
			getch();
			goto flag4;//break;
		    }
			else if(i==8)
		    {
		       //	cprintf("Enter correct choice");
			goto adminmenu;//break;
		    }
		    }
		    }//while loop closed
		    getch();
		   break;
		}//display questions closed



     else if (i==5)      //modify questions opened
		{
		   flag5 : int j,i=2;
		    disp4(2);
		    gotoxy(1,i);

		    while((j=bioskey(0))!=75)
		    {
			gotoxy(1,i);
			if(j==20480){
			    if(i<=8){
				i=i+1;
				disp4(i);//i-1
				gotoxy(1,i);
			    }
			    else{}
			}
			 else if(j==18432){
			if(i>2){
				i=i-1;
				disp4(i);//i-1
				gotoxy(1,i);
			}
			}

			 else if (j==7181){

			if(i==2)
		       {
			clrscr();
			sports_q_modify();
			getch();
		       goto flag5; //break;
		    }
			else if(i==3)
		    {
			clrscr();
			entertainment_q_modify();
			getch();
		       goto flag5;	//break;
		    }
			else if(i==4)
		    {

			clrscr();
			food_q_modify();
			getch();
		      goto flag5; //break;
		    }
			else if (i==5)
		    {
			clrscr();
			GK_q_modify();
			getch();
		       goto flag5;	//break;
		    }
			else if (i==6)
		    {
			clrscr();
			politics_q_modify();
			getch();
		       goto flag5;	//break;
		    }
			else if(i==7)
		    {   clrscr();
			TieBreaker_q_modify();
			getch();
		       goto flag5;	//break;
		    }
			else if(i==8)
		    {
		       //	cprintf("Enter correct choice");
		       goto adminmenu;	//break;
		    }
		    }
		    }//while loop closed
		    getch();
		    break;
		}  //modify closed


     else if (i==6)          //go to main menu
		{
		    clrscr();
		    getch();
		   goto MAINMENU; //break;
		}
     else
		{
		    cprintf("Enter correct choice");
		}

	       }
	       getch();
	       }

	       getch();
	       break;
     }

    else if(M==3)
	      {


		textcolor(WHITE);
	       textbackground(BROWN);
	       clrscr();
	       gotoxy(5,6);
	       cprintf("SOME CHIEF RULES TO BE FOLLOWED BY THE PLAYERS :");
	       gotoxy(5,7);
	       cprintf("________________________________________________");
	       delay(3000);
	       clrscr();
	       gotoxy(1,8);
	       cprintf("1. There are 5 rounds in this quiz.");
	       delay(3000);
	       clrscr();
	       gotoxy(1,8);
	       cprintf("2. For each correct answer +3 marks are awarded and for each wrong answer 0 marks are awarded.");
	       delay(5000);
	       clrscr();
	       gotoxy(1,8);
	       cprintf("3.VERY IMPORTANT:Each Question MUST be answered. ");
	       delay(3000);
	       clrscr();
	       gotoxy(1,8);
	       cprintf("4.No negative marks are involved in this quiz. ");
	       delay(3000);
	       clrscr();
	       gotoxy(1,8);
	       cprintf("5.[For a multiplayer quiz] At the end of the quiz if more than one individuals get the same marks as the person who has secured first position in the table , a tie breaker will be conducted. ");
	       delay(6000);
	       clrscr();
	       gotoxy(1,8);
	       cprintf("6.If even at the end of the tie breaker 2 or more individuals have the same score then they will be collectively classified as First or Second based on their performance in the tie breaker. ");
	       delay(7000);
	       clrscr();
	       gotoxy(1,8);
	       cprintf(" NOTE: if during the course of the game there exists  situation where a blank screen appears or the program remains stationary then please press ENTER slowly with a gap of one second repeatedly until the program responds");
	       delay(10000);
	       clrscr();
	       gotoxy(15,8);
	       cprintf(" BEST OF LUCK AND HOPE YOU ENJOY THE QUIZ ");
	       delay(3000);
	       clrscr();
	       gotoxy(20,12);
	       cprintf("Please Press ENTER to Test Your Knowledge");

	       getch();
	       int n;
	       player p[4];
	       clrscr();
	       gotoxy(20,12);
	       cprintf("Enter the no.of Players[max of 4] : ");
	       cin>>n;
	      while(1)
	   {
	    if(n>=1 && n<=4)
		break;
	    else
		 {
		 cprintf(" Not a valid number. Enter a valid number!");
		 //cprintf("Program Terminating...");
		 cin>>n;
		 getch();
		 //exit(0);
		  }
		   }


	       clrscr();
	       accept_player(n,p);
	       location:  int x,i=2;
		    disp(2);
		    gotoxy(1,i);

		    while((x=bioskey(0))!=75)
		    {
			gotoxy(1,i);
			if(x==20480){
			    if(i<=7){
				i=i+1;
				disp(i);//i-1
				gotoxy(1,i);
			    }
			    else{}
			}
			else if(x==18432){
			if(i>2){
				i=i-1;
				disp(i);//i-1
				gotoxy(1,i);
			}
			}
			else if (x==7181){
			clrscr();
			if(i==2){
			clrscr();
			loading();
			play_sports(n,p);
			getch();
			clrscr();
			print_score(n,p);
			//break;
			//delay(4000);
			getch();
			goto location;
			}
			else if(i==3){
			clrscr();
			loading();
			play_entertainment(n,p);
			getch();
			clrscr();
			print_score(n,p);
			//break;
			//delay(4000);

			getch();
			goto location;
			}
			else if (i==4)
			{
			clrscr();
			loading();
			play_food(n,p);
			getch();
			clrscr();
			print_score(n,p);
			//break;
			//delay(4000);
			getch();
			goto location;
			}
			else if(i==5)
			{
			clrscr();
			loading();
			play_GK(n,p);
			getch();
			clrscr();
			print_score(n,p);
			//break;
			//delay(4000);
			getch();
			goto location;
			}
			else if (i==6)
			{
			clrscr();
			loading();
			play_politics(n,p);
			getch();
			clrscr();
			print_score(n,p);
			//break;
			//delay(4000);
			getch();
			goto location;
			}

			else{
			int o = 1;
			for (int i = 1 ; i < n;i++)
			{
			   if(p[i].score==p[0].score)
			       o++;
			}

			if(o>1)
			{
			    // RISHAV LOOK HERE
			   textcolor(WHITE);
			   textbackground(BROWN);
			   clrscr();  // RISHAV LOOK HERE
			    gotoxy(2,4);
			    cprintf("Now ");
			    for(int j = 0;j<o;j++)
			    {
			       gotoxy(2,5+j);
				//RISHAV LOOK HERE
				cprintf("%s %s ",p[j].fname,p[j].lname);
			    }
			    gotoxy(10,10);
			    //RISHAV LOOK HERE
			    cprintf("will have a Tie Breaker!!!");
			    getch();
			    clrscr();
			    loading();
			    play_TieBreaker(o,p);
			    getch();
			    clrscr();
			    }
			if(n>1)
			{
			score_print(n,p);
			gotoxy(30,14);
			getch();
		       //delay(4000);
			cprintf(" Hope You Enjoyed The Quiz ");
			getch();
			}
			else
			{
			print_score(n,p);
			getch();
			//delay(4000);
			gotoxy(30,14);
			cprintf(" Hope You Enjoyed The Quiz ");
			getch();
			}
			//delay(5000);
			break;

			}
		}
			else{
			disp(i-1);
			gotoxy(1,i);
			}
		}
	       getch();
	       goto MAINMENU;
	       }

       else if(M==4)
	      {
	      credits();
	      exit(0);
	      //break;
	      }
       else
	      {
	       clrscr();
	       cprintf("Enter correct choice");
	       getch();
	       break;
	       }
    }

   getch();
}

}
/*
**************************************************************************
				End of Program
**************************************************************************
*/