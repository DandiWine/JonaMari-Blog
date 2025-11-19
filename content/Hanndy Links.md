---
Title: "Important Links That Helped Me In My studies."
---

### Accept that you can't know everything

In IT two brains are sometimes way more handy than one, your pc can be slow at times that's why you should add ram for more information to be able to take in. The same is with humans, it's better to learn from someone who knows it better than to sit hours in your room and figuring it yourself out alone.

This list is made thanks to me but also my friends in IT.

handy script for homelabs and automating bulk users

``# === CONFIGURATION ===
$csvPath = "C:\Temp\users.csv"      # path to your CSV file
$ouPath = "CN=Users,DC=ServerMoos,DC=local"  # adjust if needed
$defaultPassword = "P@ssw0rd!"      # change to a secure password

# === SCRIPT ===
$users = Import-Csv -Path $csvPath | Where-Object { $_.firstname -and $_.lastname }

foreach ($user in $users) {
    $first = $user.firstname.Trim()
    $last = $user.lastname.Trim()
    $sam = ($first + "." + $last).ToLower()
    $upn = "$first.$last@ServerMoos.local"
    $display = "$first $last"
    $dn = "CN=$display,$ouPath"

    # Build dsadd command
    $cmd = "dsadd user `"$dn`" -samid $sam -upn $upn -pwd $defaultPassword -display `"$display`" -mustchpwd no -disabled no -acctexpires never"

    Write-Output $cmd
    Invoke-Expression $cmd
}``

{{< tech_links >}}
