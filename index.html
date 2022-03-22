<!DOCTYPE html>
<html lang=”en”>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Document</title>
</head>
  
<body>

<script src="ubuntufont.js"></script>
<script src="ubuntubold.js"></script>
<script src="font1632.js"></script>
<script src="font2448.js"></script>
<script src="font3264.js"></script>
<script src="http://code.jquery.com/jquery-2.1.1.min.js"></script>
	
	
<script>
	
var elem = document.createElement('div');
elem.setAttribute("id", "divCanv");
elem.setAttribute("border", "solid black 1px");
// elem.style.cssText = 'position:absolute;width:100%;height:100%;opacity:0.3;z-index:100;background:#000';
document.body.appendChild(elem);

var canvs = document.createElement("canvas");
canvs.setAttribute("id", "canvas");
canvs.setAttribute("width", "1080");
canvs.setAttribute("height", "2176");  // 2400-112-112=2176
// canv.setAttribute("border", "solid black 1px");
document.getElementById("divCanv").appendChild(canvs); 
	
</script>
	
	
<script>
	
var cw=24; var ch=32;
var sw=4; var sh=8;
var cxi=0; var cxf=1080;
var cx=0; var cy=0;
var oh=0x41-0x20;
var data1;
	
</script>
	
	
<script>
	
var msgBuf = new ArrayBuffer(256);
var msgView = new Uint8Array(msgBuf);
var msgArr = new Uint8Array ([0x41,0x42,0x43,0x44,0x45,0x0A,0x46,data1]);
var cpr = 8; 
        
	writeChar();
	function writeChar() {
		var can = document.getElementById("canvas");
		var ctx = can.getContext('2d');
		var i=0; var j=0; var k=0;
		for (let n=0; n<cpr; n++) {
			if (msgArr[k]==0x0A) {
				i=0; j++; k++;
				if (j>50){i=0; j=0}
			} else {
				cx=(cw)*i;
				cy=(ch)*j;
				oh=msgArr[k]-0x20;
				putChar();
				i++; k++;
				if (i>25){i=0; j++;}
				if (j>50){i=0; j=0;}
			}
		}
		if (i>25){i=0; j++;}
		if (j>50){i=0; j=0;}
		cx=(cw)*i; 
		cy=(ch)*j;
		ctx.fillStyle = "blue";
		ctx.fillRect(cx-24, cy, 2, 32);
	}
	alert('2');
	// var cb = new Uint8Array ([0x80,0x40,0x20,0x10,0x08,0x04,0x02,0x01]);
	// putChar();
	function putChar() {
		var can = document.getElementById("canvas");
		var ctx = can.getContext('2d');
		var imgData = ctx.createImageData(cw, ch);
		var fontBuf = new ArrayBuffer(cw*4*ch);
		var fontView = new Uint8Array(fontBuf);
		var cb = new Uint8Array ([0x80,0x40,0x20,0x10,0x08,0x04,0x02,0x01]);
		var fb; var k=0;
		for (let i=0; i<(cw/8)*ch; i++) { 
			for (let j=0; j<8; j++) {
				fb = ubuntufont[(cw/8)*ch*oh+i] & cb[j]; 
				if (fb) {
					fontView[k+0] = 0x00;
					fontView[k+1] = 0x00;
					fontView[k+2] = 0x00;
					fontView[k+3] = 0xFF;
					k+=4;
				} else {
					fontView[k+0] = 0xFF;
					fontView[k+1] = 0xFF;
					fontView[k+2] = 0xFF;
					fontView[k+3] = 0xFF;
					k+=4;
				}
			}
		}
			for (let i=0; i<cw*4*ch; i++) {
				imgData.data[i] = fontView[i];
			}
			ctx.putImageData(imgData,cx,cy);  
	}
	
</script>
	
	
<script>
	
driveFormater();
function driveFormater() {
var driveBuf = new ArrayBuffer(128*1024*1024);
var driveView = new Uint8Array(driveBuf);
 // Master Boot Record 1MB
        driveView[0x0000010B+0x0B] = 0x00; // partition1 address LSB 0x00008000
	driveView[0x0000010B+0x0C] = 0x08; // partition1 address     8*(16*16*16) sector no.
	driveView[0x0000010B+0x0D] = 0x00; // partition1 address     8*16*16*16*512 Bytes
	driveView[0x0000010B+0x0E] = 0x00; // partition1 address MSB 16*16*16*16*16*16 = 0x00100000
	driveView[0x000001FE+0x00] = 0xAA; // signature
	driveView[0x000001FF+0x01] = 0x55; // 1MB
// Partition Volume Boot Record 1MB
	driveView[0x00100000+0x0B] = 0x00; // no of bytes per sector
	driveView[0x00100000+0x0C] = 0x02; // 2*256=512
	driveView[0x00100000+0x0D] = 0x08; // no of sectors per cluster 8
	driveView[0x00100000+0x0E] = 0x00; // no of reserve sectors
	driveView[0x00100000+0x0F] = 0x08; // 8*256=2024 sectors = 0x100000 Bytes offset of FAT1
	driveView[0x00100000+0x10] = 0x02; // no of FAT 2
	driveView[0x00100000+0x24] = 0x00; // no of sectors in each fat
	driveView[0x00100000+0x25] = 0x00; // 2024 sectors
	driveView[0x00100000+0x26] = 0x08; // 
	driveView[0x00100000+0x27] = 0x00; // 
	driveView[0x00200000+0x0C] = 0x02; // no of cluster before root directory 2
// FAT1 1MB
	driveView[0x00200000+0x00] = 0xF8; // FAT1 1MB
	driveView[0x00200000+0x01] = 0xFF; // 
	driveView[0x00200000+0x02] = 0xFF; // 
	driveView[0x00200000+0x03] = 0x0F; // 
	driveView[0x00200000+0x04] = 0xFF; // fixed
	driveView[0x00200000+0x05] = 0xFF; // 
	driveView[0x00200000+0x06] = 0xFF; // 
	driveView[0x00200000+0x07] = 0xFF; // 
	driveView[0x00200000+0x04] = 0x0F; // end of cluster
	driveView[0x00200000+0x05] = 0xFF; // 
	driveView[0x00200000+0x06] = 0xFF; // 
	driveView[0x00200000+0x07] = 0xFF; // 
// FAT2 1MB
	driveView[0x00300000+0x00] = 0xF8; // FAT2 1MB
	driveView[0x00300000+0x01] = 0xFF; // 
	driveView[0x00300000+0x02] = 0xFF; // 
	driveView[0x00300000+0x03] = 0x0F; // 
	driveView[0x00300000+0x04] = 0xFF; // fixed
	driveView[0x00300000+0x05] = 0xFF; // 
	driveView[0x00300000+0x06] = 0xFF; // 
	driveView[0x00300000+0x07] = 0xFF; // 
	driveView[0x00300000+0x04] = 0x0F; // end of cluster
	driveView[0x00300000+0x05] = 0xFF; // 
	driveView[0x00300000+0x06] = 0xFF; // 
	driveView[0x00300000+0x07] = 0xFF; //
// root directory 8MB
	driveView[0x00400000+0x01] = 0x41; // directory
	driveView[0x00400000+0x02] = 0x42; // 8*2024 sectors
	driveView[0x00400000+0x03] = 0x43; // 16192 sectors
	driveView[0x00400000+0x04] = 0x20; // 8MB
	driveView[0x00400000+0x05] = 0x20; //
	driveView[0x00400000+0x06] = 0x20; //
	driveView[0x00400000+0x07] = 0x20; //
	driveView[0x00400000+0x08] = 0x54; //
	driveView[0x00400000+0x09] = 0x58; //
	driveView[0x00400000+0x0A] = 0x54; //
	driveView[0x00400000+0x0B] = 0xFF; //
	driveView[0x00400000+0x0C] = 0xFF; //
	driveView[0x00400000+0x0D] = 0xFF; //
	driveView[0x00400000+0x0E] = 0xFF; //
	driveView[0x00400000+0x0F] = 0xFF; //
	driveView[0x00400000+0x10] = 0xFF; //
	driveView[0x00400000+0x11] = 0xFF; //
	driveView[0x00400000+0x12] = 0xFF; //
	driveView[0x00400000+0x13] = 0xFF; //
	driveView[0x00400000+0x14] = 0x80; // HO cluster no of data
	driveView[0x00400000+0x15] = 0x00; // 0x1000000+0x1000000+0x1000000+0x1000000+0x8000000=0xC000000
	driveView[0x00400000+0x16] = 0xFF; //
	driveView[0x00400000+0x17] = 0xFF; //
	driveView[0x00400000+0x18] = 0xFF; //
	driveView[0x00400000+0x19] = 0xFF; //
	driveView[0x00400000+0x1A] = 0x00; // LO cluster no of data
	driveView[0x00400000+0x1B] = 0x00; //
	driveView[0x00400000+0x1C] = 0xFF; //
	driveView[0x00400000+0x1D] = 0xFF; //
	driveView[0x00400000+0x1E] = 0xFF; //
	driveView[0x00400000+0x1F] = 0xFF; //
	
	driveView[0x00500000+0x20] = 0xFF; //
	driveView[0x00600000+0x21] = 0xFF; //
	driveView[0x00700000+0x22] = 0xFF; //
	driveView[0x00800000+0x23] = 0xFF; //
	driveView[0x00900000+0x24] = 0xFF; //
	driveView[0x00A00000+0x24] = 0xFF; //
	driveView[0x00B00000+0x24] = 0xFF; //
// data 128MB-12MB = 116MB
	driveView[0x00C00000+0x00] = 0x41; // data
	driveView[0x00C00000+0x01] = 0x42; // data
	driveView[0x00C00000+0x02] = 0x43; // data
	driveView[0x00C00000+0x03] = 0x44; // data
	driveView[0x00C00000+0x04] = 0x44; // data
	driveView[0x00C00000+0x05] = 0x46; // data
	driveView[0x00C00000+0x06] = 0x47; // data
	driveView[0x00C00000+0x07] = 0x48; // data
        
      // driveView[0x00C00000+0x08] = 0x42; // data
       data1 = driveView[0x00C00000+0x03]; // data
	
}
	
</script>
	
	
<script>  

function download() {
	
let link = document.createElement('a');  
link.download = 'hello.txt';  
let blob = new Blob(['Hello, world!'], {type: 'text/plain'});  
let reader = new FileReader();     
reader.onload = function() {  
  link.href = reader.result;
  link.click();
  document.body.removeChild(link);
};
reader.readAsDataURL(blob);
	
}
	
	
	function download2() {
	
                  var element = document.createElement('a');
                  element.setAttribute('href','data:text/plain; charset=utf-8, ' + encodeURIComponent('abc 123'));
                  element.setAttribute('download', 'abc.txt');
                  // link.setAttribute('download', 'image.jpg');
                  document.body.appendChild(element);
                  element.click();
                  document.body.removeChild(element);
	
	}

download3();
function download3() {
  
    let canvasImage = document.getElementById('canvas2').toDataURL('image/png', 1.0);
    let imageUrl = "https://cdn.pixabay.com/photo/2017/06/05/07/58/butterfly-2373175_1280.png"
	
    // this can be used to download any image from webpage to local disk
    let xhr = new XMLHttpRequest();
    xhr.responseType = 'blob';
    xhr.onload = function () {
        let a = document.createElement('a');
        a.href = window.URL.createObjectURL(xhr.response);
        a.download = 'image.png';
        a.style.display = 'none';
        document.body.appendChild(a);
        a.click();
        a.remove();
      };
      // xhr.open('GET', canvasImage); // This is to download the canvas Image
      xhr.open('GET', 'imageUrl');
      xhr.send();
  
  }

</script>  
        
	
<script>
	
function download4() {
  
    let canvasImage = document.getElementById('canvas2').toDataURL('image/png', 1.0);
    
    // this can be used to download any image from webpage to local disk
    let xhr = new XMLHttpRequest();
    xhr.responseType = 'blob';
    xhr.onload = function () {
        let a = document.createElement('a');
        a.href = window.URL.createObjectURL(xhr.response);
        a.download = 'image.png';
        a.style.display = 'none';
        document.body.appendChild(a);
        a.click();
        a.remove();
      };
     xhr.open('GET', canvasImage); // This is to download the canvas Image
      xhr.send();
  
  }
	
</script>
<script>
</script>
</body>
</html>
