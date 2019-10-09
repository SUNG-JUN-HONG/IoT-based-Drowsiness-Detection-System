# IoT-based-Drowsiness-Detection-System
A drowsiness detection sysyem based on processing electroencephalogram(EEG) data using FFT technique and a linear algorithm to compute Power Spectrum Density to identify the status of a driver. The system is capable of operating both in local and onlone modes and alert the driver with a Audio-Visual feedback to prevent accidents. 

<table>
  <tr align="center"><td><img src = 'img/system.jpg' width="50%" ></td></tr>
</table>

<H1>1.Hardware </H1>
A non-invasive commerical bluetooth EEG sensor <br>
An industrial grade tablet running on Windows 10 IoT Enterprise<br>
A headband for mounting the sensor with a set of dry electrodes<br>

<table>
  <tr align="center"><td> <img src ='img/eegsensor.jpg' width="50%" height="50%"> </td> <td> <img src='img/mt7000.jpg'> </td></tr>
</table>

<H2> 1.1 Sensor Location </H2>
<table>
  <tr><td> <img src = 'img/sensorlocation.jpg'> </td></tr>
</table>

<H1> 2. Software </H1>
.Net Framework, C# <br>
Microsoft Azure (Event Hub, Stream Analytics) <br>
Microsoft Power Bi (Data Visualization) <br>

<H1> 3. System Overview </H1>
<table>
  <tr><td> <img src = "img/systemdesign.PNG'> </td></tr>
</table>
(1) Sensor (headset + EEG sensor) <br>
(2) Tablet running on Windows 10 IoT Enterprise OS (Local Mode) <br>
(3) Azure + Power Bi (Online Mode) <br>

<H2> 3.1 FFTW Wrapper - libfftw3-3.dll </H2>

FFTW is a C subroutine library for computing the discrete Fourier transform (DFT) in one or more dimensions, of arbitrary input size, and of both real and complex data.<br>

FFTW wrapper written by Tamas Szalay:<br>
https://github.com/tszalay/FFTWSharp/tree/master/FFTWtest<br>
<br>
FFTW Original SOurce:<br>
http://www.fftw.org/download.html<br>
