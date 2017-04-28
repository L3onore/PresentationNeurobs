scenario = "False memory - encoding session"; # name of this scenario file

pcl_file = "3013065.02.MRI.Encoding.v1.pcl"; # direct to the correct pcl file


#default_font = "Comic Sans MS"; # can choose all types of fonts you want
default_font = "Calibri";
default_font_size = 30;
default_text_color = 235,235,235; # nearly white, but not entirely, better for eyes
default_text_align = align_left;

active_buttons = 15; #say how many you have
button_codes = 1, 2, 3,4,5,6,7,8,9,10,11,12,13, 14,15;# the numbers in the settings, the number under the #sign
# 1 = left mouse button
# 2 = right mouse button
# 3 = enter
# 4 = left
# 5 = right
# 6= leftup
# 7 = rightup
# 8 = A
# 9 = s
# 10 = d
# 11 = j
# 12 = k
# 13 = l
# 14 = up
# 15 = down


begin; # there is no end

#input screen
picture {
} p_default;

picture { text { caption = "ask for info"; } 
			  t_info_1; x=0; y=100;
		    text { caption = " ";} 
			  t_info_2; x=0; y=0;
			 text { caption = "Press [ENTER] to confirm or [ESC] to stop the program!"; } t_info_3; x=0; y=-200;
			} p_info;

# Instructions
picture { text { caption = "	Instructie";font_size = 15;} t_instruc_1;
			   x = 0; y = 0;
			 text { caption = "	Je gaat zometeen woorden een voor een op het scherm zien. \n
										Probeer elk woord zo goed mogelijk te onthouden! \n
										De woorden zijn onderverdeeld in lijsten waarin je elk woord 2 keer zult zien. 
																			 									 "; } t_instruc_2;
				x = 0; y = -50;
} p_instruction;

picture { text { caption = "	Instructie";font_size = 15;} t_instruc_11;
			   x = 0; y = 0;
			 text { caption = "	Morgen, in sessie 2, vragen we je hoeveel woorden je nog onthouden hebt. \n
Let dus goed op en probeer zo veel mogelijk woorden te onthouden! 
																			 									 "; } t_instruc_12;
				x = 0; y = -50;
} p_instruction4;





picture { text  { caption = "Na elke lijst verschijnt een balk op het scherm. \n
										De bedoeling is dat je na elke lijst aangeeft in hoeverre je stemming is veranderd, \n
										ten opzichte van aan het begin van het experiment. \n
										Je kunt met de pijltjes toetsen van links naar rechts over de balk schuiven. \n
										Je hebt hiervoor 3 seconden de tijd. \n \n
										
										
										Dan verschijnt er weer een balk. \n
										Hier vragen we je hoeveel woorden je van de vorige lijst denkt te kunnen onthouden. \n
										Je kunt met de pijltjes toetsen naar rechts over de balk schuiven. \n
										Je hebt hiervoor 3 seconden de tijd. \n \n
										Gebruik altijd ENTER om te bevestigen.
								";font_size = 20; } t_instruc_4;
				x = 0; y = -50;
} p_instruction2;

picture { text  { caption = " Veel succes!";} t_instruc_7;
				x = 0; y = 0;
				
			 text  { caption = " Heb je nog vragen? Stel ze nu aan de onderzoeker! \n 
										Druk op Enter om te beginnen"; } t_instruc_8;
				x = 0; y = -50;
} p_instruction3;


picture {  text { caption = " *** Volgende lijst ***";} t_instruc_9;
				 x = 0; y = 100;
				} p_lijst;


#The word gets presented here, the word Target gets replacd by all target words, or stimuli from the txt file
picture { text { caption =" +  "; }t_target;  x= -100;y=  150;
          text { caption =" +  "; }t_target2; x=  100;y=  150;  
			 text { caption =" +  "; }t_target3; x= -100;y=    0; 
			 text { caption =" +  "; }t_target4; x=  100;y=    0; 
			 text { caption =" +  "; }t_target5; x= -100;y= -150; 
			 text { caption =" +  "; }t_target6; x=  100;y= -150; 
			
}p_target;


#duration of target
trial {
   picture p_target;
   time = 0;
   duration = 6000;
}t_trial;

#optional break
picture { text { caption ="Pause"; } t_pause; x=0;y=0;
}p_pause;

#First slider (mood)
picture {
# the line
box { color = 255,255,255; height = 3; width = 350; };
x = 0; y = 0;
# the cursor
box { color = 255,0,0; height = 50; width = 3; };
x = 0; y = 0;
# text
text { caption = "Relatief verdrietiger"; font_size = 24; };
x = -360; y = 0;
text { caption = "Relatief vrolijker"; font_size = 24; };
x = 360; y = 0;
text { caption = "Wat is je stemming op dit moment?"; font_size = 36; };
x = 0; y = 250;
} lines;

#Second slider (meta)
picture {
# the line
box { color = 255,255,255; height = 3; width = 350; };
x = 0; y = 0;
# the cursor
box { color = 255,0,0; height = 50; width = 3; };
x = 0; y = 0;
# text
text { caption = "Geen enkele"; font_size = 24; };
x = -360; y = 0;
text { caption = "Allemaal"; font_size = 24; };
x = 360; y = 0;
text { caption = "Hoeveel woorden denk je dat je van deze lijst hebt onthouden?"; font_size = 36; };
x = 0; y = 250;
} metalines;


# ----- What was the color?------#
picture {  
#Blue
#box { color = 0,0,255; height = 100; width = 100; };
#x = -350; y = -200;
#Red
#box { color = 255,0,0; height = 100; width = 100; };
#x = 350; y = -200;


# text
text { caption = "Blauw"; font_size = 36; font_color = 0,0,255;};
x = -300; y = 0;
text { caption = "Blauw"; font_size = 36; font_color = 0,0,255; };
x = 300; y = 0;
text { caption = "Rood"; font_size = 36; font_color = 255,0,0;};
x = 300; y = -200;
text { caption = "Rood"; font_size = 36; font_color = 255,0,0; };
x = -300; y = -200;

text { caption = "Welke kleur kwam het meeste voor in deze lijst?"; font_size = 36; };
x = 0; y = 150;

text { caption = "â†‘Pijltje omhoogâ†‘ " ; font_size =36; font_color = 250,250,250; background_color = 0,0,255; };
x = 0; y = 0;
text { caption = "â†“Pijltje omlaagâ†“" ; font_size =36; font_color = 250,250,250; background_color = 255,0,0;};
x = 0; y = -200;



}p_colorquest;




# fixation cross between lists
picture { 
box { color = 255,255,255; height = 20; width = 3; };
x = 0; y = 0;
box { color = 255,255,255; height = 3; width = 20; };
x = 0; y = 0;
} fix;
#duration of fixation cross
trial {
   picture fix;
   time = 0;
   duration = 1000;
}t_fix;

# ITI fixation cross (between words)
picture { 
box { color = 255,255,255; height = 20; width = 3; };
x = 0; y = 0;
box { color = 255,255,255; height = 3; width = 20; };
x = 0; y = 0;
} fix2;
#duration of fixation cross
trial {
   picture fix;
   time = 0;
   duration = 1000;
}t_fix2;

# ITI blank (between words
picture {  text { caption = " ";} t_instruc_10;
				 x = 0; y = 0;
				} p_ITI;
#duration of blank
trial {
   picture p_ITI;
   time = 0;
   duration = 250;
}t_ITI;

#ending screen
picture { text  { caption = "Bedankt! \n Probeer alle woorden zo goed mogelijk te onthouden! \n
											Haal aub de onderzoeker uit de andere ruimte";} t_bye;
				x = 0; y = 0;
			 				
} p_goodbye;



# proberen om twee woorden tegelijk te laten zien!



