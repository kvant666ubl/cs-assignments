class Sensor {
    public:
        int pin;
        int val;
    
        Sensor(int);      
        void printData(); 
        void getConfig(); 
};
void setup() {
  Serial.begin(9600);
  
}

Sensor::Sensor(int pin_) {
    pin = pin_;
}

void Sensor::getConfig() {
   Serial.print("Pin | "); 
   Serial.println(pin);
}

void Sensor::printData() {
     val = digitalRead(pin);
     Serial.print("Data | "); 
     Serial.println(val);
}

void loop() {
    Sensor digital(3);
    digital.getConfig();
    digital.printData();
}
