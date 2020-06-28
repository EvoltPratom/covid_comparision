# Covid Comparision

(In windows use Powershell)

<code>wget -o covid.zip https://github.com/EvoltPratom/covid_comparision/archive/master.zip</code>


Extract the files

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


