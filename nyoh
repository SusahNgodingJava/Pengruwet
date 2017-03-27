<?php
include "../subkoneksi.php";

$sql = "SELECT nama, nbi, passw FROM mahasiswa"; 
mysqli_select_db($con,$db_name);

$ambildata = mysqli_query($con,$sql);
if(!$ambildata )
{
  die('Gagal' . mysqli_error($con));
}
echo "<div id='kotak1'>Nama Mahasiswa</div><div id='kotak2'>NBI</div><div id='kotak2'>Passw</div><div id='wrapper'>";
while($row = mysqli_fetch_array($ambildata, MYSQLI_ASSOC))
{
    echo "<br><div id='kotak3'>{$row['nama']}</div>"."<div id='kotak4'>{$row['nbi']}</div>"."<div id='kotak4'>{$row['passw']}</div>";
}
echo "</div>";
?>
