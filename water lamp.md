# container1


#include<reg52.h>

sbit led1=P1^0;
sbit led2=P1^1;
sbit led3=P1^2;
sbit led4=P1^3;
sbit led5=P1^4;
sbit led6=P1^5;
sbit led7=P1^6;
sbit led8=P1^7;
void delay_ms(unsigned char i);

void main()
{
	while(1)
	{
		led1=0;
		delay_ms(1000);
		led1=1;
		delay_ms(1000);

		led2=0;
		delay_ms(1000);
		led2=1;
		delay_ms(1000);

		led3=0;
		delay_ms(1000);
		led3=1;
		delay_ms(1000);

		led4=0;
		delay_ms(1000);
		led4=1;
		delay_ms(1000);

		led5=0;
		delay_ms(1000);
		led5=1;
		delay_ms(1000);

		led6=0;
		delay_ms(1000);
		led6=1;
		delay_ms(1000);

		led7=0;
		delay_ms(1000);
		led7=1;
		delay_ms(1000);

		led8=0;
		delay_ms(1000);
		led8=1;
		delay_ms(1000);
	}
}
void delay_ms(unsigned char i)
{
	unsigned char count_ms,count_us;

	for(count_ms=0;count_ms<i;count_ms++)
		for(count_us=0;count_us<151;count_us++);

}
