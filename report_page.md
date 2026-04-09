# Lab0 — 1-page report (Setup & Hello Deep Learning)

## Thiết lập môi trường
- Sử dụng Anaconda tạo environment Python 3.10 và cài đặt thư viện từ requirements.txt (numpy, pandas, sklearn, torch, ...).

## Các bước kiểm tra
- Chạy `check_env.py` để kiểm tra môi trường → import thành công, torch hoạt động, device = CPU.
- Chạy `run_smoke_test.py` để test pipeline Deep Learning (MLP) → train và evaluate qua 3 epoch.

## Kết quả
- Mô hình đạt test_acc ≈ 0.74 sau 3 epochs, loss giảm dần.
- Sinh đầy đủ outputs: logs, loss_curve.png và checkpoint model.

## Vấn đề & cách xử lý
- Gặp lỗi OMP (libiomp5md.dll) do xung đột thư viện → xử lý bằng cách cài PyTorch qua conda để đồng bộ môi trường.
- Đảm bảo activate đúng conda env trước khi chạy.