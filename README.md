# Covid Comparision

(In windows use Powershell)

<code>wget -o covid.zip https://github.com/EvoltPratom/covid_comparision/archive/master.zip</code>


Extract the files

<code>Expand-Archive covid.zip -DestinationPath covid</code>

Run the following

<code> pip install -r requirements.txt </code>

<code>python main.py</code>

You can also use the file corona.py as a module

eg:

```sh
>>> import corona as cr
>>> cr.get_stats('Nepal')
{'country': 'Nepal', 'tot-cases': '12,309', 'new-cases': '', 'tot-death': '28 ', 'new-death': '', 'tot-recovered': '2,834', 'serious': '', 'active': '9,447', 'tot-tests': '504,910'}
>>>
```

```sh
>>> help(cr.get_cases)
get_cases(c_name, type_of_data)
    type of data can be the following
    graph-active-cases-total
    graph-cases-daily
    graph-deaths-daily

>>> cr.get_cases('nepal','graph-cases-daily')
{'Feb15': '0', 'Feb16': '0', 'Feb17': '0', 'Feb18': '0', 'Feb19': '0', 'Feb20': '0', 'Feb21': '0', 'Feb22': '0', 'Feb23': '0', 'Feb24': '0', 'Feb25': '0', 'Feb26': '0', 'Feb27': '0', 'Feb28': '0', 'Feb29': '0', 'Mar01': '0', 'Mar02': '0', 'Mar03': '0', 'Mar04': '0', 'Mar05': '0', 'Mar06': '0', 'Mar07': '0', 'Mar08': '0', 'Mar09': '0', 'Mar10': '0', 'Mar11': '0', 'Mar12': '0', 'Mar13': '0', 'Mar14': '0', 'Mar15': '0', 'Mar16': '0', 'Mar17': '0', 'Mar18': '0', 'Mar19': '0', 'Mar20': '0', 'Mar21': '0', 'Mar22': '0', 'Mar23': '1', 'Mar24': '0', 'Mar25': '1', 'Mar26': '0', 'Mar27': '1', 'Mar28': '1', 'Mar29': '0', 'Mar30': '0', 'Mar31': '0', 'Apr01': '0', 'Apr02': '1', 'Apr03': '0', 'Apr04': '3', 'Apr05': '0', 'Apr06': '0', 'Apr07': '0', 'Apr08': '0', 'Apr09': '0', 'Apr10': '0', 'Apr11': '0', 'Apr12': '3', 'Apr13': '2', 'Apr14': '2', 'Apr15': '0', 'Apr16': '0', 'Apr17': '14', 'Apr18': '1', 'Apr19': '0', 'Apr20': '0', 'Apr21': '11', 'Apr22': '3', 'Apr23': '3', 'Apr24': '1', 'Apr25': '0', 'Apr26': '3', 'Apr27': '0', 'Apr28': '2', 'Apr29': '3', 'Apr30': '0', 'May01': '2', 'May02': '0', 'May03': '16', 'May04': '0', 'May05': '7', 'May06': '17', 'May07': '2', 'May08': '1', 'May09': '7', 'May10': '1', 'May11': '24', 'May12': '83', 'May13': '26', 'May14': '6', 'May15': '18', 'May16': '14', 'May17': '14', 'May18': '80', 'May19': '27', 'May20': '25', 'May21': '30', 'May22': '59', 'May23': '68', 'May24': '19', 'May25': '79', 'May26': '90', 'May27': '114', 'May28': '156', 'May29': '170', 'May30': '189', 'May31': '171', 'Jun01': '239', 'Jun02': '288', 'Jun03': '201', 'Jun04': '334', 'Jun05': '278', 'Jun06': '323', 'Jun07': '213', 'Jun08': '314', 'Jun09': '324', 'Jun10': '278', 'Jun11': '250', 'Jun12': '448', 'Jun13': '273', 'Jun14': '425', 'Jun15': '451', 'Jun16': '380', 'Jun17': '586', 'Jun18': '671', 'Jun19': '426', 'Jun20': '331', 'Jun21': '421', 'Jun22': '535', 'Jun23': '538', 'Jun24': '629', 'Jun25': '434', 'Jun26': '593', 'Jun27': '554'}
>>>
```
Notice in this function the 1st character of country name should be in lower case


