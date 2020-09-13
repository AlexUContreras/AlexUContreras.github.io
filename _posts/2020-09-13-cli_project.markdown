---
layout: post
title:      "Cli Project "
date:       2020-09-13 22:31:43 +0000
permalink:  cli_project
---


So for my first project, I wanted to keep it simple, and as we progress in the course challenge myself more and more. So for my CLI project, I used an API called Kanye-Rest. The API puts out random Kanye quotes in a hash. The hardest part of the project for me was calling the API  into my CLI class. I knew how to call it and store it into the variable but that all. I did research and figure out a little more but was still lost. I decided to schedule a 1 on 1 meeting with my cohort lead and I'm so happy I did.
She helped me understand the steppes I was missing and made me understand why we people things that we put. So now I had my CLI working and every time you call it gave you a Kanye quote when the user inputs "Y" for yes. When the user put "N" for no it told the user to have a good day, but if the user inputted something that wasn't Y or N it printed for them to have a nice day witch is what i didn't want. I wanted it to make the user try again, so i refactored my code to make it a while loop.

```
def menu
        puts "Would you like a random Kanye Quote? Y/N"
        while answer = gets.chomp.upcase
            case answer
            when "Y"
                puts "Quote: #{Quote.all.first.quote}"
                break
            when "N"
                puts "Have a good day!"
                break
            else 
                puts "Error, Try again"
            end
        end
    end
```

Simply but im proud of this code that I wrote.
