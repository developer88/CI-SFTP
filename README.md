# CI-SFTP

SFTP Library for CodeIgniter. 

## Setup
Copy all files and folders to your application directory.

Change settings in config/sftp.php

## Usage

Get list of files:

	$this->load->library('sftp'); // initialize library
	$this->sftp->connect(); // connect to sftp server. if autoconnect option set to false
	print_r($this->sftp->files_list('/some_dir/')); //get list of files


Download a file:

	$this->load->library('sftp'); // initialize library
	$this->sftp->connect(); // connect to sftp server. if autoconnect option set to false
	echo $this->sftp->download('/some_dir/some_file'); //get list of files

## Changes
### 0.1.0
* Initial release