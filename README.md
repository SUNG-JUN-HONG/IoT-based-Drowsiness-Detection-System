# IoT-based-Drowsiness-Detection-System (Capstone Project)
A drowsiness detection sysyem based on processing electroencephalogram(EEG) data using FFT technique and a linear algorithm to compute Power Spectrum Density to identify the status of a driver. The system is capable of operating both in local and online modes ,and alerts the driver with a Audio-Visual feedback to prevent accidents. Originally, the project was a final-year Capstone project for Mechatroincs Systems Enginnering (MSE) Program at Simon Fraser University (SFU) with a team of four 4th year undergraudate students in 2019. After the final semester, Sung Jun Hong and Nicholas Wong(a Graduate Student at SFU MSE program) have continuded and are responsible for the development of the project <br>

<h3> Contributors </h3>
<table align = "center" width = "50%" >
  <tr> <th> Participants </th> <th> Periods </tr>
  <tr><td> <b> Capstone Team: Brainiac System </b> <br> Sung Jun Hong <br> Dishan Fernando <br> M.Hashim Shahzad <br> Faruque Al Mahumud <br> Keith McLaughlin </td> 
  <td> Jan 2019 ~ August 2019 </td> </tr>
  <tr> <td> Sung Jun Hong (C#, Azure, .Net Framework, Power Bi) <br> Nicolas Wong (Drowsiness detection linear algorithm, MATLAB prototype) </td> <td> Sep 2019 ~ Dec 2019 </td> </tr>
</table>
  
<br>

<h3> Screenshot </h3>
<table align="center">
  <tr align="center"><td><img src ='img/demogif.gif'></td></tr>
  <tr> <td><img src = 'img/system.jpg' width="50%" ></td></tr>
</table>
<hr>

<h1>1. Hardware</h1>
<ul type ="disk">
  <li>A non-invasive commerical bluetooth EEG sensor </li>
  <li>An industrial grade tablet running on Windows 10 IoT Enterprise</li>
  <li>A headband for mounting the sensor with a set of dry electrodes</li>
</ul>
<table>
  <tr align="center"><td> <img src ='img/eegsensor.jpg' width="300px" height="300px"> </td> <td> <img src='img/mt7000.jpg'> </td></tr>
</table>

<h2> Sensor Location </h2>
<table align="center">
  <tr><td> <img src = 'img/sensorlocation.jpg'> </td></tr>
</table>
<hr>

<h1>2. Software</h1>
<ul type="disk">
  <li>.Net Framework, C#</li>
  <li>Microsoft Azure (Event Hub, Stream Analytics)</li>
  <li>Microsoft Power Bi (Data Visualization) </li>
</ul>

<h1>3. System Overview</h1>
<table>
  <tr><td><img src='img/systemdesign.png'></td></tr>
</table>
(1) Sensor (headset + EEG sensor) <br>
(2) Tablet running on Windows 10 IoT Enterprise OS (Local Mode) <br>
(3) Azure + Power Bi (Online Mode) <br>

<H2> 3.1 FFTW Wrapper - libfftw3-3.dll </H2>
FFTW is a C subroutine library for computing the discrete Fourier transform (DFT) in one or more dimensions, of arbitrary input size, and of both real and complex data.<br>
<br>
FFTW wrapper written by Tamas Szalay:<br>
https://github.com/tszalay/FFTWSharp/tree/master/FFTWtest<br>
<br>
FFTW Original Source:<br>
http://www.fftw.org/download.html<br>

<H2> 3.2 ThinkGear SDK for .NET - Thinkgear.dll </H2>
Neurosky Windows Developer Tools 3.2 : https://store.neurosky.com/products/pc-developer-tools <br>
Development Guide and API Reference: http://developer.neurosky.com/docs/doku.php?id=thinkgear.net_sdk_dev_guide_and_api_reference
