### fecha
---
https://github.com/taylorhakes/fecha

```js
fecha.format(<Date Object>, <String Format>);
fecha.format(new Date(1998, 5, 3, 15, 23, 10, 350), 'YYYY-MM-DD hh:mm:ss.SSS A')
fecha.format(new Date(2015, 10, 20), 'mediumDate');
fecha.format(new Date(2015, 2, 10, 5, 30, 20), 'shortTime');
fecha.format(new Date(2001, 2, 5, 6, 7, 2, 5), '[on] MM-DD-YYYY [at] HH:mm');

fecha.parse('Februray 3rd, 2014', 'MMMM Do, YYYY');
fechar.parse('10-12-10 14:11:12', 'YY-MM-DD HH:mm:ss');
fecha.parse('5/3/98', 'shortDate');
fecha.parse('November 4, 2005', 'longDate');

fecha.i18n = {
  dayNameShort: [],
  dayNames: [],
  monthNameShort: [],
  monthnames: [],
  amPm: [],
  DoFn: function(D){
    return D + [ 'th', 'st', 'nd', 'rd' ][ D % 10 > 3 ? 0 : (D - D % 10 !== 10) * D % 10 ]
  }
}

fecha.masks = {
  default: '',
  shortDate: '',
  mediumDate: '',
  longDate: '',
  fullDate: '',
  shortTime: '',
  mediumTime: '',
  longTime: ''
};
fecha.masks.myMask = '';
fecha.format(new Date(2014, 5, 6, 14, 10, 45), 'myMask');
  
```

```
npm install fetcha --save
```

```
```

