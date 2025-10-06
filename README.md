SteelFlow: Real-Time Ladle ID and Location Tracking for SMS-1 & SMS-2 Optimization

Unzip and open a terminal in the project folder.

Create venv and install dependencies:

python -m venv venv
source venv/bin/activate   # on Windows: venv\\Scripts\\activate
pip install -r requirements.txt


Run server:

python server/app.py


In another terminal run the simulator:

python edge_client.py


Open the dashboard at: http://localhost:5000

Notes & next steps I can do for you (pick any):

Replace the edge simulator with a real edge inference script: YOLOv8 detection + OCR wrapper (Tesseract/EasyOCR) tuned for ladle images.

Add WebSocket/Socket.IO for instant dashboard pushes instead of polling.

Add image storage + operator verification UI for low-confidence reads.

Create a React-based dashboard with floorplan visualization and analytics.

Build Docker images and test docker-compose end-to-end.
