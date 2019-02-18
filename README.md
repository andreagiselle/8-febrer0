# 8-febrero
int rojo = 3;
int verde = 4;
int ambar = 5;
int t1;
int t2;
int t3;

void setup() {
  Serial.begin(9600);
  
  Serial.println("¿Cuánto tiempo rojo?");
  while(Serial.available() ==0){
    
  }
  t1=Serial.parseInt();
  pinMode(rojo, OUTPUT); 

  Serial.println("¿Cuánto tiempo verde?");
  while(Serial.available() ==0){
    
  }
  t2=Serial.parseInt();
  pinMode(verde, OUTPUT);

  Serial.println("¿Cuánto tiempo ambar?");
  while(Serial.available() ==0){
    
  }
  t3=Serial.parseInt();
  pinMode(ambar, OUTPUT);
}

void loop() {
  digitalWrite(rojo, HIGH);
  delay(t1);
  digitalWrite(rojo, LOW);
  delay(t1);
  digitalWrite(verde, HIGH);
  delay(t2);
  digitalWrite(verde, LOW);
  delay(t2);
  digitalWrite(ambar, HIGH);
  delay(t3);
  digitalWrite(ambar, LOW);
  delay(t3);
}
