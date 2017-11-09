#include "mbed.h"

DigitalIn mybutton(USER_BUTTON);
DigitalOut myled(LED1);

int main() {
  while(1) {
    if (mybutton == 0) { // Button is pressed
        myled=1;
    } else {
        myled=0;
    }

  }
}
