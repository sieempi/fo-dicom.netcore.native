# fo-dicom.netcore.native
fo-dicom dotnet core native codecs windows linux osx pinvoke playground


**Supported Transfer Syntaxes:**

UID     | Name
-------- | ---
1.2.840.10008.1.2.4.50 | JPEG Baseline (Process 1)
1.2.840.10008.1.2.4.51 | JPEG Baseline (Processes 2 & 4)
1.2.840.10008.1.2.4.57 | JPEG Lossless, Nonhierarchical (Process 14)
1.2.840.10008.1.2.4.70 | JPEG Lossless, Nonhierarchical, First-Order Prediction (Process 14 [SV1])
1.2.840.10008.1.2.4.80 | JPEG-LS Lossless Image Compression
1.2.840.10008.1.2.4.81 | JPEG-LS Lossy (Near-Lossless) Image Compression
1.2.840.10008.1.2.4.90 | JPEG 2000 Image Compression (Lossless Only)
1.2.840.10008.1.2.4.91 | JPEG 2000 Image Compression

**Usage:** 

Dicom.Imaging.Codec.TranscoderManager.SetImplementation(NETCoreTranscoderManager.Instance);
DicomFile.Open("foo.dcm").Clone(DicomTransferSyntax.JPEG2000Lossless);
