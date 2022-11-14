# korea-covid19-hosp-data

Hospitalization data from official sources:

* Daily report in Korean, [Sample page](https://www.kdca.go.kr/board/board.es?mid=a20501010000&bid=0015&list_no=718247&cg_code=&act=view&nPage=1)). Sunsetted on 2022-10-30.
* From 2022-11-01, *weekly* Wednesday report of hospitalization stats contain the daily figures (1 week delay).
* For most up-to-date daily stats without delay, refer to the [Stat page (Korean)](https://ncov.kdca.go.kr/bdBoardList_Real.do?brdId=1&brdGubun=11&ncvContSeq=&contSeq=&board_id=&gubun=)

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
* This will no longer be updated in this page for foreseeable future given potential discrepancy arising from antigen tests

The [beds.csv](beds.csv) contains the hospitalization information based on severity level
* The official government report figures are updated daily
* The report also contains bed capacity, which is not included in the figure. Only filled bed counts are added
* From 2022-11-01, this stats is also published only weekly.

The files will be updated weekly.
