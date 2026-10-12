<h1>Digital Forensics with Autopsy</h1>


<h2>Description</h2>
I utilized Autopsy, a digital forensics software, to investigate a scenario-based lab where an employee is suspected of stealing proprietary and confidential data from their company. The task involved conducting a digital forensic examination of the employee's corporate workstation and presenting any relevant findings in a report, as per the company's request.
<br />


<h2>Utilities Used</h2>

- <b>Autopsy</b> 

<h2>Environments Used </h2>

- <b>Windows 10</b>

<h2>Autopsy walk-through:</h2>

<p align="center">
Launch Autopsy: <br/>
<img src="https://i.imgur.com/TFZd2YG.png" height="90%" width="90%" alt="Launch Autopsy from Desktop"/>
<br />
<br />
Select "New Case":  <br/>
<img src="https://i.imgur.com/CSaW9jF.png" height="90%" width="90%" alt="Create New Case"/>
<br />
<br />
Enter the Case Information: <br/>
<img src="https://i.imgur.com/HK4Rnvn.png" height="90%" width="90%" alt="Case Name and Directory"/>
<br />
<br />
<img src="https://i.imgur.com/pggay9I.png" height="90%" width="90%" alt="Case Number"/>
<br />
<br />
Add a Data Source (Select Host System):  <br/>
<img src="https://i.imgur.com/wMr266r.png" height="90%" width="90%" alt="Select Host"/>
<br />
<br />
Add a Data Source (Select Data Source Type):  <br/>
<img src="https://i.imgur.com/8bsv39x.png" height="90%" width="90%" alt="Data Source Type"/>
<br />
<br />
Add a Data Source (Select Data Source Path):  <br/>
<img src="https://i.imgur.com/a57PwWP.png" height="90%" width="90%" alt="Data Source Path"/>
<br />
<br />
Add a Data Source (Configure Ingest, Use Default Settings):  <br/>
<img src="https://i.imgur.com/jYuEmwG.png" height="90%" width="90%" alt="Configure Ingest"/>
<br />
<br />
Finish Adding Data Source:  <br/>
<img src="https://i.imgur.com/W1oV81M.png" height="90%" width="90%" alt="Finish Adding Data Source"/>
<br />
<br />
Identify Potential Evidence:  <br/>
</p>
<p>
  a.	To uncover evidence, I initiated a search on John Smith’s computer hard drive using Autopsy. Upon expanding the directory, I promptly identified numerous carved and deleted files of interest. Notably, these files contained instructions on untraceable Bitcoin transactions and Crypto laundering techniques. Additionally, deleted files labeled “Business Strategy” and “Drilling Methodology” hinted at potential evidential significance.
</p>
<p align="center">
<img src="https://i.imgur.com/gTnmlDK.png" height="90%" width="90%" alt="Directory Overview"/>
<br />
<br />
</p>
<p>
  b.	I extended my examination of John Smith’s hard drive by filtering results for PDF files. Despite being deleted, I successfully located and accessed files titled “Business Strategy,” “Drilling Methodology,” and “Oil Company Data Strategy.” The former two were marked as “CONFIDENTIAL Restricted,” while the latter was labeled “Confidential – No Release.” After extraction, I stored the files in: C:\Users\LabUser\Desktop\Evidence Files\John Smith\Export, and generated hash values for each file using MD5 and SHA-256 hashing algorithms. 
</p>  
<p align="center">
<img src="https://i.imgur.com/k21eF2D.png" height="90%" width="90%" alt="Business Strategy Extract"/>
<br />
<br />
<img src="https://i.imgur.com/a5Qx7Yh.png" height="90%" width="90%" alt="Business Strategy Hash"/>
<br />
<br />
<img src="https://i.imgur.com/7gZS4lG.png" height="90%" width="90%" alt="Drilling Methodology Extract"/>
<br />
<br />
<img src="https://i.imgur.com/QvKxF2H.png" height="90%" width="90%" alt="Drilling Methodology Hash"/>
<br />
<br />
<img src="https://i.imgur.com/Zjxe0Jg.png" height="90%" width="90%" alt="Oil Strategy Extract"/>
<br />
<br />
<img src="https://i.imgur.com/ZNHavRB.png" height="90%" width="90%" alt="Oil Strategy Hash"/>
<br />
<br />
</p>  
<p>
  c.	I also extracted all PDF files concerning hiding Bitcoin transactions and crypto laundering, and I hashed these files as well.
</p>  
<p align="center">
<img src="https://i.imgur.com/eHV7VKR.png" height="90%" width="90%" alt="Transaction Mixer Extract"/>
<br />
<br />
<img src="https://i.imgur.com/8Hmj3wv.png" height="90%" width="90%" alt="Transaction Mixer Hash"/>
<br />
<br />
<img src="https://i.imgur.com/Y99cywg.png" height="90%" width="90%" alt="6 Ways Bitcoin Extract"/>
<br />
<br />
<img src="https://i.imgur.com/XW3nhxd.png" height="90%" width="90%" alt="6 Ways Bitcoin Hash"/>
<br />
<br />
<img src="https://i.imgur.com/oi6sEy5.png" height="90%" width="90%" alt="Bitcoin Anon Extract"/>
<br />
<br />
<img src="https://i.imgur.com/dTJv3mQ.png" height="90%" width="90%" alt="Bitcoin Anon Hash"/>
<br />
<br />
<img src="https://i.imgur.com/o4IcimP.png" height="90%" width="90%" alt="Crypto Laundering Extract"/>
<br />
<br />
<img src="https://i.imgur.com/FPkTUrE.png" height="90%" width="90%" alt="Crypto Laundering Hash"/>
<br />
<br />
</p>
<p>
  d.	Next, I combed through the files in the “Deleted Files” directory, uncovering two additional .jpg files containing diagrams possibly representing proprietary company data. After extraction, I also hashed these files. 
</p>
<p align="center">
<img src="https://i.imgur.com/HcqEYB4.png" height="90%" width="90%" alt="Oil Co Conf1 Extract"/>
<br />
<br />
<img src="https://i.imgur.com/6efAKtZ.png" height="90%" width="90%" alt="Oil Co Conf1 Hash"/>
<br />
<br />
<img src="https://i.imgur.com/gw6RUb5.png" height="90%" width="90%" alt="Oil Co Conf2 Extract"/>
<br />
<br />
<img src="https://i.imgur.com/aJaU9GG.png" height="90%" width="90%" alt="Oil Co Conf2 Hash"/>
<br />
<br />
Summary:  <br/>
</p>
<p>
  a.	In total there were nine files of interest located on John Smith’s computer. The most interesting files were the “Business_Strategy.pdf,” “Drilling Methodology.pdf,” and “Oil Company data strategy.pdf” files. This is due to these three files as clearly being labeled confidential and John Smith should not have access to such files. It should also be noted that of those three files, the “Business_Strategy.pdf” file and the “Drilling Methodology” file were deleted from John Smith’s computer. John Smith has clearly violated the NDA and AUP of the company by being in possession of these files.
<br />
<br />
b.	There were also four files relating to Bitcoin transactions. These files appeared to be articles that covered various topics regarding Bitcoin such as how to make untraceable Bitcoin transactions, how to use Bitcoin anonymously, how to hide “dirty” Bitcoins, and even crypto laundering. This is of particular interest because it suggests that John Smith was looking for how to make untraceable Bitcoin transactions. This should be investigated further since John Smith was in possession of proprietary company information. It could mean that John Smith was motivated by financial gain.
<br />
<br />
c.	The last two files of interest were .jpg files that could be proprietary data. These files appear to be diagrams of equipment and processes used by the company. They were also deleted files, suggesting that either John no longer needed them or should not have had them to begin with and attempted to hide the files. See the photo below for the files that were extracted from John Smith’s hard drive.
<br />
<br />
</p>
<p align="center">
<img src="https://i.imgur.com/wqvntXj.png" height="80%" width="80%" alt="Summary of Files Found"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
