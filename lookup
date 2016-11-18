<?
//----- Open Socket connection to WhoIs server of Libya (whois.nic.ly) using port (43)
$fp = fsockopen("whois.nic.ly", 43);

//----- Add "\r\n" to your domain to signifying the end of a line of text and the start of a new line.
$ly_domain = "Sites.ly"."\r\n";

//----- Send the data to whois server.
fwrite($fp, $ly_domain);

//----- Listen for incoming data, and save it in string variable, in our case is ($whois_info).
while (!feof($fp)) {
	$whois_info .= fgets($fp, 128);
}

//----- Print ($whois_info) variable, OR check it to specify whether the domain registered or not.
echo $whois_info;
?>
