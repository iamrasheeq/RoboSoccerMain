char t;
int speedCar = 150;
int ls = 5;
int rs = 10;

int a = 6;
int b = 7;
int c = 8;
int d = 9;

void forward();
void backward();
void left();
void right();
void stopCar();

void setup() {
   
  
   Serial.println("You're connected via Bluetooth");
   pinMode(a,OUTPUT);   
   pinMode(b,OUTPUT);   
   pinMode(c,OUTPUT);  
   pinMode(d,OUTPUT);   
   pinMode(ls,OUTPUT);
   pinMode(rs,OUTPUT);

  digitalWrite(ls,speedCar);
  digitalWrite(rs,speedCar);
  
   Serial.begin(9600);
   

}
void loop() {


  
  

  if(Serial.available())
  {
  t = Serial.read();
  Serial.println(t);
  }


  if(t == 'F')
  {
    forward();
     t = 'S';
   }
   else if(t == 'B')
   {
      backward();
      t = 'S';
    }else if(t == 'L')
   {
      left();
      t = 'S';
    }else if(t == 'R')
   {
      right();
      t = 'S';
    }else if(t == 'S')
   {
      stopCar();
      
    }else if(t == '0')
   {
       speedCar = 100;
    }else if(t == '1')
   {
       speedCar = 140;
    }else if(t == '2')
   {
       speedCar = 150;
    }else if(t == '3')
   {
       speedCar = 165;
    }else if(t == '4')
   {
       speedCar = 180;
    }else if(t == '5')
   {
       speedCar = 190;
    }else if(t == '6')
   {
       speedCar = 205;
    }else if(t == '7')
   {
       speedCar = 216;
    }else if(t == '8')
   {
       speedCar = 225;
    }else if(t == '9')
   {
       speedCar = 240;
    }else if(t == 'q')
   {
       speedCar = 255;
    }


//  switch (t){
//
//     case 'F':
//      forward();
//      t = 'S';
//      break;
//      
//     case 'B':
//      backward();
//      t = 'S';
//      break;
//
//
//     case 'L':
//      left();
//      t = 'S';
//      break;
//      
//     case 'R':
//      right();
//      t = 'S';
//      break;
//
//
//     case 'S':
//      stopCar();
//      
//      break;
//      
//    case '0':
//        speedCar = 100;
//        break;
//      case '1':
//        speedCar = 140;
//        break;
//      case '2':
//        speedCar = 153;
//        break;
//      case '3':
//        speedCar = 165;
//        break;
//      case '4':
//        speedCar = 178;
//        break;
//      case '5':
//        speedCar = 191;
//        break;
//      case '6':
//        speedCar = 204;
//        break;
//      case '7':
//        speedCar = 216;
//        break;
//      case '8':
//        speedCar = 229;
//        break;
//      case '9':
//        speedCar = 242;
//        break;
//      case 'q':
//        speedCar = 255;
//        break;
//      
//    
//    }

    
      
   delay(25);


}



void forward(){

      
        
      digitalWrite(a,LOW);
      digitalWrite(b,HIGH);
      digitalWrite(c,HIGH);
      digitalWrite(d,LOW);

      analogWrite(ls,speedCar);
      analogWrite(rs,speedCar);
  
  }

void backward(){

      
  
      digitalWrite(a,HIGH);
      digitalWrite(b,LOW);
      digitalWrite(c,LOW);
      digitalWrite(d,HIGH);

      analogWrite(ls,speedCar);
      analogWrite(rs,speedCar);
  }
void left(){
  
      
      
      digitalWrite(a,LOW);
      digitalWrite(b,HIGH);
      digitalWrite(c,LOW);
      digitalWrite(d,HIGH);

      analogWrite(ls,speedCar);
      analogWrite(rs,speedCar);
  }

void right(){

   
      
      digitalWrite(a,HIGH);//HIGH
      digitalWrite(b,LOW);
      digitalWrite(c,HIGH);
      digitalWrite(d,LOW);

      analogWrite(ls,speedCar);
      analogWrite(rs,speedCar);
  }


void stopCar(){

      
      digitalWrite(a,LOW);//HIGH
      digitalWrite(b,LOW);
      digitalWrite(c,LOW);
      digitalWrite(d,LOW);

      analogWrite(ls,speedCar);
      analogWrite(rs,speedCar);
  }
