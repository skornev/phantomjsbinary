# phantomjsbinary
phantomjs binary with download 
Linux phantomjs binary for Debain 7 with download support.
OnLoadFinished still says "fail", but download file should appear in the current directory.




page.onFilePicker = function(oldFile)
{
    console.log('onFilePicker(' + oldFile + ') called');
    return 'InvoiceReport.pdf';
}
page.onDownloadFinished = function(status)
{
    console.log('onDownloadFinished(' + status + ')');
    phantom.exit(1);
}
page.onLoadFinished = function(status)
{
    console.log('onLoadFinished(' + status + ')');
}

