# OfficeDevPnP.Core.Framework.TimerJobs
## Classes
|**Class**|**Description**|
|:-----|:-----|
|[TimerJob](OfficeDevPnP.Core.Framework.TimerJobs.TimerJob.md)|Abstract base class for creating timer jobs (background processes) that operate against SharePoint sites. These timer jobs are designed to use the CSOM API and thus can run on any server that can communicate with SharePoint.|
|[TimerJobRun](OfficeDevPnP.Core.Framework.TimerJobs.TimerJobRun.md)|Class that holds the state information that's being stored in the web property bag of web that's being "processed"|
|[TimerJobRunEventArgs](OfficeDevPnP.Core.Framework.TimerJobs.TimerJobRunEventArgs.md)|Event arguments for the TimerJobRun event|
|[TimerJobRunHandler](OfficeDevPnP.Core.Framework.TimerJobs.TimerJobRunHandler.md)|TimerJobRun delegate|
