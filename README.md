# Dicom-Viewer

![App Preview](/Example.png)

DICOM viewer with basic medical image processing functionalities such as contrast adjustment, brightness control, zoom, and filtering. Built to assist in visualizing and enhancing medical images for diagnostic purposes.

##1. Core Features (Loading & Display):
 DICOM File Parsing Reads metadata and pixel data using dicomParser. Supports drag-and-drop and file selection via a button. Image Rendering Converts raw pixel data into a displayable image using <canvas>. Applies DICOM parameters (rescale slope/intercept, photometric interpretation).
##2. Image Adjustments  Windowing (Window Level/Width) 
Interactive sliders to adjust center (WC) and width (WW). Reset button to restore default DICOM values. Brightness/Contrast Sliders for fine-tuning brightness (±) and contrast (%). Quick presets (e.g., "Bright," "Dark," "High Contrast"). Color Inversion Toggle between black-on-white and white-on-black. 
##3. Interaction Tools  Zoom Zoom in/out (buttons or mouse wheel). 
Mouse-centered zoom for precise navigation. Zoom reset. Pan (Moving the Image) Toggleable pan mode to drag the image. Rotation & Flip Rotate clockwise/counterclockwise (90°). Flip horizontally/vertically. 
##4. Analysis Tools  Magnifying Glass (Loupe) Displays a 9x9 grid zoom around the hovered pixel. Highlights the center pixel in red. Pixel Information Real-time display of coordinates (X/Y) and Hounsfield value. DICOM Metadata Shows critical tags (patient name, ID, modality, image size, etc.). Full list of DICOM tags in a scrollable panel. 
##5. UI & Usability  Global Reset "Reset All" button to restore default settings. Loading Overlay Displays a progress message during file loading. Responsive Design Adjustable panels (metadata/image) and mouse/keyboard-friendly controls. 
##6. Advanced Features (Custom Logic)  Auto Windowing Calculates optimal WC/WW if tags are missing, based on pixel histogram. Signed/Unsigned Pixel Support Handles signed pixels (two's complement) for CT scans. Photometric Interpretation Adapts rendering for MONOCHROME1 (native inversion) and MONOCHROME2.
