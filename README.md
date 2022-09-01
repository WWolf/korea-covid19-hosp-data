# korea-covid19-hosp-data

Hospitalization data from official sources (daily report in Korean, [Sample page](https://www.kdca.go.kr/board/board.es?mid=a20501010000&bid=0015&list_no=718247&cg_code=&act=view&nPage=1)). For most daily current stats, refer to the [English page](http://ncov.mohw.go.kr/en/bdBoardList.do?brdId=16&brdGubun=161&dataGubun=&ncvContSeq=&contSeq=&board_id=)

The [hospitalization.csv](hospitalization.csv) contains the following information:
* **New Hospital admissions (daily)** (from 2021-11-01)
* **Hospitalizations with moderate to severe symptoms**
  - Patients receiving isolated treatment through high flow therapy, respirator, ECMO (extracorporeal membrane oxygenation), and CRRT (continuous renal replacement therapy) (from 2020-03-28)
  - Stats sourced from [SNU ARIC COVID-19](https://sites.google.com/view/snuaric/data-service/covid-19/covid-19-data?authuser=0) for data before 2021-11-01.
* Date refers to the reported day (00:00), so a data point of 2022-01-15 corresponds to admissions, patient status of 2022-01-14.

The [weekly_icu.csv](weekly_icu.csv) contains weekly information on
* **Hospital admissions with moderate to severe symptoms (weekly)**
  - Above daily figures are the number of patients, whereas this figure is the new admissions
* **Hospital admissions (weekly)**
  - This is redundant statistics of the aggregate of daily new hospital admissions
* Note that the date is reported date, and there is 3 day difference (2022-08-30 report means 2022-08-21 to 2022-08-27 weekly period)

The [testing.csv](testing.csv) contains testing information (continuation of now discontinued ARIC SNU project)
* The official government report figures are revised daily up to one week
* This is updated semi-weekly, so there will be small discrepancies of figures to the most up-to-date figure (1 week after the report) depending on the date


The files will be updated weekly.
