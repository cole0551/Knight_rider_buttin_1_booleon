# Knight_rider_buttin_1_booleon
int switchState = 0;
bool lightstate= false;

void setup() {
 pinMode (3,OUTPUT);
 pinMode (4,OUTPUT);
 pinMode(5,OUTPUT); 
 pinMode(2,INPUT);
  
  

}

void loop() {
  switchState = digitalRead(2);
  delay(100);
  if(switchState==HIGH){
    lightstate=!lightstate;
     delay(100);
  }

  
  if(lightstate==true){  
  digitalWrite (4,LOW);
  digitalWrite (3,LOW);
  digitalWrite (5,LOW);
  digitalWrite (7,LOW);
  digitalWrite (6,LOW);
  }
  else{
digitalWrite (4,HIGH);
digitalWrite (3,HIGH);
digitalWrite (5,HIGH);
digitalWrite (7,HIGH);
digitalWrite (6,HIGH);
  }
}
