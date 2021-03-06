[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
[![Build Status](https://travis-ci.org/VencejoSoftware/ooDatetime.svg?branch=master)](https://travis-ci.org/VencejoSoftware/ooDatetime)

# ooDatetime - Object pascal datetime library
Library manipulate date/time data types as objects

### Documentation
If not exists folder "code-documentation" then run the batch "build_doc". The main entry is ./doc/index.html

### Example
```pascal
var
  DateTimeSpan: IDateTimeSpan;
begin
  DateTimeSpan := TDateTimeSpan.Create(TDaySpan.NewByDate(Now), TTimeSpan.NewByTime(Now));
  with DateTimeSpan do
  begin
    ShowMessage(Format('Day: %d/%d/%d Time: %d:%d:%d.%d', [DaySpan.Number, Ord(DaySpan.Month.Number),
      DaySpan.Year.Number, TimeSpan.Hour, TimeSpan.Minute, TimeSpan.Second, TimeSpan.Millisecond]));
  end;
end;
```

### Demo
Before all, run the batch "build_demo" to build proyect. Then go to the folder "demo\build\release\" and run the executable.

## Built With
* [Delphi&reg;](https://www.embarcadero.com/products/rad-studio) - Embarcadero&trade; commercial IDE
* [Lazarus](https://www.lazarus-ide.org/) - The Lazarus project

## Contribute
This are an open-source project, and they need your help to go on growing and improving.
You can even fork the project on GitHub, maintain your own version and send us pull requests periodically to merge your work.

## Authors
* **Alejandro Polti** (Vencejo Software team lead) - *Initial work*