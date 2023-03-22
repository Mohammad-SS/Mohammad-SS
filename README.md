<div align="center">
<img src="https://raw.githubusercontent.com/Mohammad-SS/Mohammad-SS/main/helloworld.gif" align="center" style="width: 100%" />
</div>  
  

### <div align="center">I'm Mohammad Azimi , a Backend Developer . You need me ?! Feel free to DM💬 me in Linkedin </div>  
[![Linkedin: Mohammad1996Azimi](https://img.shields.io/badge/-mohammad1996azimi-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/mohammad1996azimi/)](https://www.linkedin.com/in/mohammad1996azimi/)

<br/>  


```python
from humans import status
from datetime import date
from past import memories
from routines import create_good_memories , wake_up , code , drink_coffe , sleep 


class Mazimi(ME):
    '''
    This class extends myself in a very very short code !
    '''
    # Personal information
    first_name = "Mohammad"
    middle_name = "Bagher"
    last_name = "Azimi"
    alias = "MAzimi"
    personality = "ESTJ" # Based on MBTI test 

    # Skills 
    main_skills = ["Python" , "Django" , "DRF" ]
    secondary_skills = ["HTML","CSS" , "JS" , "PHP" , "Docker" ]
    used_to_be = ["Freelancer" ,"Fullstack Developer in Esra and Apptech"]

    # Trivia ! 
    time_zone = "Asia/Tehran"
    goal = "Be Happy ! Any where , Any Time !"
    good_memories = [memory for memory in memories if memory.my_status == status.HAPPY ]

    def life_cycle(self):
        '''
        It shows how i spend my every F...ing Days !
        '''

        while self.status == status.ALIVE :

            weekday = date.today().weekday()
            if weekday in ["3" , "4"] : # 3:Thursday and 4:Friday
                self.good_memories.append(create_good_memories()) # Maybe a short trip :)
                continue

            wake_up()
            code() 
            drink_coffe(choices=["Latte" , "Americano"]) # Americano will be choosed if we have bugs !
            code()
            sleep()
        
        return self.good_memories # When i pass away , only my good memories will remain :)

    @classmethod
    def test_sleep_hour(cls , sleep_datetime , wakeup_datetime):
        '''
        what will happen if my sleep quality be bad !?
        Args : 
         - sleep_datetime : datetime object
         - wakeup_datetime : datetime object
        '''
        sleep_quality = (sleep_datetime - wakeup_datetime).hours
        assert sleep_quality > 7 , "Today I need to drink more coffe !"
        assert sleep_quality < 10 , "I lost this day ! AZ SHANBE ISHALA :D"
    

```


