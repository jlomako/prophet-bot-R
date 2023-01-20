# prophet-bot-R

Bot written in R that reads data from <a href="https://github.com/jlomako/hospital-occupancy-tracker">hospital-occupancy-tracker</a> repository, then runs prophet and calculates predictions for <a href = "https://github.com/jlomako/Montreal-ER">Montreal-ER</a> web app (visit app <a href="https://jlomako.shinyapps.io/Montreal_ER/">here</a>)

[![get-predictions-in-R](https://github.com/jlomako/prophet-bot-R/actions/workflows/prophet_bot_R.yml/badge.svg)](https://github.com/jlomako/prophet-bot-R/actions/workflows/prophet_bot_R.yml)

### notes to myself:
* Holiday effects for Quebec were added manually as prophet function <code>add_country_holidays</code> is not supported in R 4.2. (holiday package was removed from CRAN). 
* updated yml-workflow, still doesn't run on ubuntu because of some error with curl (in renv) 
* doesn't work on ubuntu with <code>DESCRIPTON</code> either
* runs every 2nd day at 1:25 pm local time
* this bot has been replaced by a faster bot that runs on ubuntu and does exactly the same but in python <a href = "https://github.com/jlomako/prophet-bot">prophet-bot</a>
* disabled workflow
