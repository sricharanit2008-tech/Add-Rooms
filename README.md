MINI PROJECT HANDBOOK ASSIGNMENT
Course Code & Title: 25ITT11 – C Programming
Module: Add Room Module

Function Definition
The function addRoom() is a user-defined function used to collect room details from the user and store them permanently in a text file. It adds a new room record to the hotel management system.
Meaning of the Code

1. FILE *fp = fopen("rooms.txt", "a");
   Opens the file in append mode to add new room details without deleting existing data.

2. if (fp == NULL)
   Checks whether the file is opened successfully.

3. struct Room r;
   Declares a structure variable to store room details.

4. scanf("%d", &r.roomNo);
   Reads the room number from the user.

5. scanf("%s", r.type);
   Reads the room type (Single/Double/Suite).

6. scanf("%f", &r.price);
   Reads the price per night.

7. r.isBooked = 0;
   Sets the default booking status as available.

8. fprintf(fp, "%d %s %.2f %d", ...);
   Writes the room data into the file.

9. fclose(fp);
   Closes the file after writing.

10. printf("Room added successfully");
    Displays a success message to the user.
