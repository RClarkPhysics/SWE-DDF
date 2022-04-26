# SWE-DDF
This Repository includes a new application of DDF to the field of Fluid Physics, specifically the Shallow Water Equations. In an Effort to make DDF a useful tool in the field of weather forecasting we have adapted DDF to handle the Shallow Water Equations (SWE). We tackle the interesting problem of handling a reduced dimensional data set, meaning we are trying to study a data set that doesn't observe all obesrvable quantities in a physical system. Since it is impossible to measure the infinite number of data points across all of the ocean, we must restrict ourselves to a limited number of observations; to recapture the lost information in this process, we use time delay embedding to learn the lost statistical information in the data (We have found that the inclusion of time delay embedding has a dramatic effect on the forecasting performance as long as a proper time delay is chosen!). DDF could have exciting uses in the area of regional weather forecasting. We exemplify this effect by generating a 10 by 10 grid of SWE data and then training and forecasting a reduced dimensional 3 by 3 grid with DDF.

The DDF Folder is the standard DDF which contains the standard Gaussian+Polynomial(1st order) python script and a jupyternotebook guide on how to use it. It also contains an example of using it on a 10 by 10 grid. Here is a video showcasing DDF's forecasting ability (the black grid) against the Shallow Water (the colorful surface):

https://user-images.githubusercontent.com/54558570/165237147-11ce9bc9-ac32-49d1-a16a-f4c5141f1624.mp4

The Time Delay Embedding DDF Folder contains the TDE DDF python script as well as the jupyter notebook that guides users through it. Test data is included and an example folder is also included which contains a graph, video, and two text files of the results of a successful test. Here is a video of the regional weather forecasting ability of DDF using time delay embedding on a 3 by 3 corner of the 10 by 10 grid (The black outline is the prediction, the colorful tiles are the true SWE data):

https://user-images.githubusercontent.com/54558570/164692112-e4673e7d-05c8-4c6e-998f-7b5237f180f0.mp4

The Shallow Water Equations themselves with Wind Forcing:

How we Generated the SWE (include a link to the papers method):
