# README

This is FreeDoc, the new Doctolib !

Here is what you should know about this fantastic project

# Versions
* Ruby version 2.5.1
* Rails version 5.2.4

# Relation between tables
* Doctor - Patient :            n - n
* Doctor - Appointment :        1 - n
* Patient - Appointment :       1 - n
* Doctor - City :               n - 1
* Patient - City :              n - 1
* Appointment - City :          n - 1
* Doctor - Specialty :          n - n (creation of SpectialtyDoctor as join table)
* Doctor - SpecialtyDoctor :    1 - n
* Specialty - SpecialtyDoctor : 1 - n

# Run tests
* $ tp Doctor.all
* $ tp Specialty.all
* $ tp Patient.all
* $ tp SpecialtyDoctor.where(doctor_id:11)

# Gem
* table_print: You can use "tp" to visualize the information as tables
* faker: To create a fake database

