## This is my Trivy html template

**How to get Trivy Report**

1) Download html template to local -> https://github.com/kantapit123/trivy-report/blob/main/html.tpl

2) Copy file to `/usr/local/bin`
```
sudo cp html.tpl /usr/local/bin/html.tpl
```

3) Build your image

4) Scan with output html format
```
trivy image --format template --template "@/usr/local/bin/html.tpl" -o report.html <image>:<tag>
```
--- Done ✅ ---

If you want PDF

5) Go to https://html2pdf.com/ 

6) Upload your html and Download PDF file
