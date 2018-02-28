# tanya

The included python codes, help our Raspberry Pi to communicate with the MySQL Database. 

The first file: Hostel.py updates the entry/exit time in the database of the detected card holder
(through a RFID sensor attached to the Raspberry Pi)

The second File: sql.py
This files creates a new entry in the Mess-Coupons table, when a student pays the vendor the mess fees, adding the designated number of coupons that a user purchased.
From then onwards, whenever the user swipes his/her card on the RFID sensor connected to Raspberry Pi, if coupons are left, one coupon is deducted.
This deduction takes place from the Breakfast coupons, Lunch coupons, Evening Tea coupons or Dinner coupons, according to the current system time.
If the coupons are less than required, the buzzer goes off and no updates are made.
