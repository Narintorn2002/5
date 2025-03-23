<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="utf-8">
    <title>หน่วยงานส่วนภูมิภาคในสังกัดสำนักวิจัยและพัฒนาการป่าไม้</title>
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
    <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
    <script src="https://unpkg.com/leaflet-control-geocoder/dist/Control.Geocoder.js"></script>
    <style>
        body {
            margin: 0;
            display: flex;
            height: 100vh;
            flex-direction: row;
        }

        #map {
            flex-grow: 1;
        }

        #sidebar {
            width: 25%;
            background: linear-gradient(135deg, #f9f9f9, #e3f2fd);
            overflow-y: auto;
            padding: 10px;
            box-shadow: -2px 0 8px rgba(0, 0, 0, 0.2);
            font-size: 14px;
            font-family: Arial, sans-serif;
        }

        h3 {
            margin-top: 0;
            font-size: 16px;
            color: #1e88e5;
            text-align: center;
            font-weight: bold;
        }

        .checkbox-item {
            margin: 10px 0;
            background: #ffffff;
            padding: 8px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            display: flex;
            align-items: center;
        }

        input[type="checkbox"] {
            margin-right: 10px;
            cursor: pointer;
            flex-shrink: 0;
        }

        .checkbox-text {
            color: #555;
            text-decoration: none;
            cursor: pointer;
            flex-grow: 1;
        }

        #search-box {
            position: fixed;
            top: 20px;
            left: 50px;
            z-index: 9999;
            background-color: white;
            padding: 5px 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        #search-box input {
            width: 200px;
            padding: 5px;
            font-size: 14px;
        }

        #search-box button {
            padding: 5px;
            background-color: #1e88e5;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        #search-box button:hover {
            background-color: #1565c0;
        }

        .link-container {
            position: relative;
            padding-left: 20px;
            display: none;
            background-color: #f0f0f0;
            padding: 10px;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            margin-top: 5px;
        }

        .link-container::before {
            content: "";
            position: absolute;
            top: 50%;
            left: 0;
            width: 2px;
            height: 50px;
            background: blue;
            transform: translateY(-50%);
        }

        .link-container.show {
            display: block;
        }

        .link-container a {
            display: block;
            background-color: #1e88e5;
            color: white;
            padding: 10px;
            border-radius: 5px;
            text-align: center;
            text-decoration: none;
            font-weight: bold;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
            transition: background-color 0.3s;
        }

        .link-container a:hover {
            background-color: #1565c0;
        }

        .tree-info-container {
            display: none;
            background-color: #dff0d8;
            padding: 10px;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            margin-top: 5px;
        }

        .tree-info-container.show {
            display: block;
        }
    </style>
</head>
<body>
    <div id="map"></div>

    <div id="sidebar">
        <h3>หน่วยงานส่วนภูมิภาคในสังกัดสำนักวิจัยและพัฒนาการป่าไม้</h3>
        <form id="checkbox-list"></form>
    </div>

    <div id="search-box">
        <input type="text" id="search-input" placeholder="ค้นหาสถานี..." onkeydown="handleSearch(event)">
        <button onclick="searchStation()">ค้นหา</button>
    </div>

    <script>
        var map = L.map('map').setView([14.0, 100.0], 5.5);

        var osm = L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
            maxZoom: 18,
            attribution: '© OpenStreetMap'
        }).addTo(map);

        var satellite = L.tileLayer('https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}', {
            maxZoom: 18,
            attribution: '© ESRI, Maxar, Earthstar Geographics'
        });

        var baseMaps = {
            "แผนที่ถนน (OSM)": osm,
            "แผนที่ดาวเทียม": satellite
        };

        L.control.layers(baseMaps).addTo(map);

        var geojsonFeatures = {
            "type": "FeatureCollection",
            "features": [
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk1",
                        "name": "ศูนย์วนวัฒนวิจัยที่1 เชียงใหม่",
                        "description": "ที่อยู่ : อ.เมือง จ.เชียงใหม่<br>ชื่อหัวหน้า : นางอภิระมน ฐิติชยาภรณ์<br>เบอร์ติดต่อ : 086-5868877",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้สัก (Tectona grandis)",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้ยาง (Hevea brasiliensis)",
							"<strong>ข้อมูลพรรณไม้ 3:</strong> ไม้ยาง (Hevea brasiliensis)"
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [98.950291, 18.809096]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk2",
                        "name": "ศูนย์วนวัฒนวิจัยที่2 ลำปาง",
                        "description": "ที่อยู่ : ต.บ้านหวด อ.งาว จ.ลำปาง<br>ชื่อหัวหน้า : นายศุภชัย นุชิต<br>เบอร์ติดต่อ : 089-7010497",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [99.898220, 18.631467]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk3",
                        "name": "ศูนย์วนวัฒนวิจัยที่3 กำแพงเพชร",
                        "description": "ที่อยู่ : ต.หนองปลิง อ.เมือง จ.กำแพงเพชร<br>ชื่อหัวหน้า : นายจิตรพล ไทยภักดี<br>เบอร์ติดต่อ : 081-2610519",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [99.505128, 16.562968]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk4",
                        "name": "ศูนย์วนวัฒนวิจัยที่4 กาญจนบุรี",
                        "description": "ที่อยู่ : ต.ท่าล้อ อ.ท่าม่วง จ.กาญจนบุรี<br>ชื่อหัวหน้า : นายจรัส ช่วยนะ<br>เบอร์ติดต่อ : 089-8906682",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [99.56959444, 14.00889998]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk5",
                        "name": "ศูนย์วนวัฒนวิจัยที่5 ขอนแก่น",
                        "description": "ที่อยู่ : ต.นาหนองทุ่ม อ.ชุมแพ จ.ขอนแก่น<br>ชื่อหัวหน้า : นายสุชาติ นิ่มพิลา<br>เบอร์ติดต่อ : 092-2463009",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [101.986681, 16.819352]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk6",
                        "name": "ศูนย์วนวัฒนวิจัยที่6 นครราชสีมา",
                        "description": "ที่อยู่ : ต.อุดมทรัพย์ อ.วังน้ำเขียว จ.นครราชสีมา<br>ชื่อหัวหน้า : นายนรินทร์ เทศสร<br>เบอร์ติดต่อ : 087-1026162",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [101.904102, 14.468021]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk7",
                        "name": "ศูนย์วนวัฒนวิจัยที่7 ประจวบคีรีขันธ์",
                        "description": "ที่อยู่ : ต.อ่าวน้อย อ.เมือง จ.ประจวบคีรีขันธ์<br>ชื่อหัวหน้า : นางสาวอารียาพัชร์ เพชรรัตน์<br>เบอร์ติดต่อ : 093-9969907",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [99.81493, 11.838788]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk8",
                        "name": "ศูนย์วนวัฒนวิจัยที่8 สุราษฎร์ธานี",
                        "description": "ที่อยู่ : ต.มะขามเตี้ย อ.เมือง จ.สุราษฎร์ธานี<br>ชื่อหัวหน้า : นายเอกภพ เพิ่มพูล<br>เบอร์ติดต่อ : 094-5947058",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [99.363475, 9.101511]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk9",
                        "name": "ศูนย์วนวัฒนวิจัยที่9 สงขลา",
                        "description": "ที่อยู่ : ต.ฉลุง อ.หาดใหญ่ จ.สงขลา<br>ชื่อหัวหน้า : นางสาวอารียาพัชร์ เพชรรัตน์<br>เบอร์ติดต่อ : 093-9969907",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [100.21505307, 7.1090591061]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk10",
                        "name": "ศูนย์เมล็ดพันธุ์ไม้ป่าภาคกลาง(สระบุรี)",
                        "description": "ที่อยู่ : ต.มิตรภาพ อ.มวกเหล็ก จ.สระบุรี<br>ชื่อหัวหน้า : นางสาวกรรณิการ์ ดุมา<br>เบอร์ติดต่อ : 036-341305",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [101.201862, 14.643983]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk11",
                        "name": "ศูนย์เมล็ดพันธุ์ไม้ป่าภาคตะวันออกเฉียงเหนือ(ขอนแก่น)",
                        "description": "ที่อยู่ : ต.โนนสมบูรณ์ อ.บ้านแฮด จ.ขอนแก่น<br>ชื่อหัวหน้า : นางสาวอนงคณี เรือนทิพย์<br>เบอร์ติดต่อ : 085-1274917",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [102.783177, 16.247042]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk12",
                        "name": "ศูนย์เมล็ดพันธุ์ไม้ป่าภาคใต้(สงขลา)",
                        "description": "ที่อยู่ : ต.ฉลุง อ.หาดใหญ่ จ.สงขลา<br>ชื่อหัวหน้า : นางสาวสุทิศา รวมเงาะ<br>เบอร์ติดต่อ : 081-8963412",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [100.305307, 7.011235]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk13",
                        "name": "ศูนย์เมล็ดพันธุ์ไม้ป่าภาคเหนือ(ลำปาง)",
                        "description": "ที่อยู่ : ต.บ้านหวด อ.งาว จ.ลำปาง<br>ชื่อหัวหน้า : นายศุภชัย นุชิต<br>เบอร์ติดต่อ : 089-7010597",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [99.91836171, 18.6367434]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk14",
                        "name": "สถานีวนวัฒนวิจัยทรายทอง",
                        "description": "ที่อยู่ : ต.ทรายทอง อ.บางสะพานน้อย จ.ประจวบคีรีขันธ์<br>ชื่อหัวหน้า : นางสาวอารียาพัชร์ เพชรรัตน์<br>เบอร์ติดต่อ : 093-9969907",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [99.457489, 10.990028]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk15",
                        "name": "สถานีวนวัฒนวิจัยทองผาภูมิ",
                        "description": "ที่อยู่ : ต.ท่าขนุน อ.ทองผาภูมิ จ.กาญจนบุรี<br>ชื่อหัวหน้า : นางสาวกิตยาภรณ์ ใจอารีย์<br>เบอร์ติดต่อ : 082-2144445",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [98.6520231, 14.712742]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk16",
                        "name": "สถานีวนวัฒนวิจัยท่าตูม",
                        "description": "ที่อยู่ : ต.หนองบัว อ.ท่าตูม จ.สุรินทร์<br>ชื่อหัวหน้า : นายอภิรัตน์ พิรุฬห์<br>เบอร์ติดต่อ : 081-3215965",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [103.762284, 15.3139745]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk17",
                        "name": "สถานีวนวัฒนวิจัยบ่อแก้ว",
                        "description": "ที่อยู่ : ต.บ่อหลวง อ.ฮอด จ.เชียงใหม่<br>ชื่อหัวหน้า : นายพยนต์ เรืองระยนต์<br>เบอร์ติดต่อ : 093-1363812",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [98.389079, 18.15318]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk18",
                        "name": "สถานีวนวัฒนวิจัยพิษณุโลก",
                        "description": "ที่อยู่ : ต.บ้านแยง อ.นครไทย จ.พิษณุโลก<br>ชื่อหัวหน้า : นายศุภฤกษ์ สุนทรสถิตย์<br>เบอร์ติดต่อ : 084-0333992",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [100.8877354, 16.8430662]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk19",
                        "name": "สถานีวนวัฒนวิจัยแม่กา",
                        "description": "ที่อยู่ : ต.แม่กา อ.เมือง จ.พะเยา<br>ชื่อหัวหน้า : นายพูนศักดิ์ ไชยดวงแก้ว<br>เบอร์ติดต่อ : 097-2290379",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [99.900361, 18.99653]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk20",
                        "name": "สถานีวนวัฒนวิจัยแม่สะนาม",
                        "description": "ที่อยู่ : ต.บ่อสลี อ.ฮอด จ.เชียงใหม่<br>ชื่อหัวหน้า : นายพยนต์ เรืองระยนต์<br>เบอร์ติดต่อ : 093-1363812",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [98.283297, 18.162964]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk21",
                        "name": "สถานีวนวัฒนวิจัยราชบุรี",
                        "description": "ที่อยู่ : ต.เกาะพลับพลา อ.เมืองราชบุรี จ.ราชบุรี<br>ชื่อหัวหน้า : นางสาวกมลพร ชัยวิศิษฐ์<br>เบอร์ติดต่อ : 062-9291651",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [99.7392728, 13.573348]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk22",
                        "name": "สถานีวนวัฒนวิจัยลำเภา-ลำทราย",
                        "description": "ที่อยู่ : ต.บ้านเก่า อ.เมือง จ.กาญจนบุรี<br>ชื่อหัวหน้า : นายสิทธิชัย อยู่ดี<br>เบอร์ติดต่อ : 064-1562425",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [99.3032488, 13.9716866]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk23",
                        "name": "สถานีวนวัฒนวิจัยหนองคู",
                        "description": "ที่อยู่ : ต.ทับทิน อ.สังขะ จ.สุรินทร์<br>ชื่อหัวหน้า : นางสาวสุนิศา ศรีวีระพันธ์<br>เบอร์ติดต่อ : 089-3091674",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [103.7742804, 14.6758367]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk24",
                        "name": "สถานีวนวัฒนวิจัยหมูสี",
                        "description": "ที่อยู่ : ต.หมูสี อ.ปากช่อง จ.นครราชสีมา<br>ชื่อหัวหน้า : นางสาวมนัสสุดา นันทสิริพร<br>เบอร์ติดต่อ : 081-7183381",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [101.4829842, 14.4989928]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk25",
                        "name": "สถานีวนวัฒนวิจัยห้วยทา",
                        "description": "ที่อยู่ : ต.รุ่งระวี อ.น้ำเกลี้ยง จ.ศรีสะเกษ<br>ชื่อหัวหน้า : นางสาววราพร โพธิสาร<br>เบอร์ติดต่อ : 064-7830222 , 087-0764100",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [104.4411652, 14.8743946]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk26",
                        "name": "สถานีวนวัฒนวิจัยห้วยบง",
                        "description": "ที่อยู่ : ต.บ่อหลวง อ.ฮอด จ.เชียงใหม่<br>ชื่อหัวหน้า : นายไภรเวช ศรีบุตรตา<br>เบอร์ติดต่อ : 096-3594445",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [98.427266, 18.150289]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk27",
                        "name": "สถานีวนวัฒนวิจัยหินลับ",
                        "description": "ที่อยู่ : ต.หนองกุ่ม อ.บ่อพลอย จ.กาญจนบุรี<br>ชื่อหัวหน้า : นายจรัส ช่วยนะ<br>เบอร์ติดต่อ : 089-8906682",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [99.450487, 14.211977]
                    }
                },
                {
                    "type": "Feature",
                    "properties": {
                        "id": "chk28",
                        "name": "สถานีวนวัฒนวิจัยอินทขิล",
                        "description": "ที่อยู่ : ต.อินทขิล อ.แม่แตง จ.เชียงใหม่<br>ชื่อหัวหน้า : นายไภรเวช ศรีบุตรตา<br>เบอร์ติดต่อ : 096-3594445",
                        "treeInfo": [
                            "<strong>ข้อมูลพรรณไม้ 1:</strong> ไม้ยาง (Hevea brasiliensis) ใช้ในการผลิตยางพารา...",
                            "<strong>ข้อมูลพรรณไม้ 2:</strong> ไม้สน (Pinus spp.) ใช้ในการผลิตไม้ยางพารา..."
                        ]
                    },
                    "geometry": {
                        "type": "Point",
                        "coordinates": [98.952983, 19.15298]
                    }
                }
            ]
        };

        var featureLayers = {};

        function addCheckbox(feature, layer) {
            var checkboxForm = document.getElementById("checkbox-list");

            var div = document.createElement("div");
            div.className = "checkbox-item";

            var checkbox = document.createElement("input");
            checkbox.type = "checkbox";
            checkbox.id = feature.properties.id;
            checkbox.checked = true;

            checkbox.addEventListener("change", function () {
                if (this.checked) {
                    layer.addTo(map);
                    layer.openPopup();
                } else {
                    map.removeLayer(layer);
                }

                var linkContainer = document.getElementById('station-link-' + feature.properties.id);
                if (this.checked) {
                    linkContainer.classList.add('show');
                } else {
                    linkContainer.classList.remove('show');
                }

                var treeInfoContainer = document.getElementById('tree-info-container-' + feature.properties.id);
                if (this.checked) {
                    treeInfoContainer.classList.add('show');
                } else {
                    treeInfoContainer.classList.remove('show');
                }
            });

            var spanText = document.createElement("span");
            spanText.className = "checkbox-text";
            spanText.innerHTML = feature.properties.name;
            spanText.addEventListener("click", function () {
                var latlng = L.latLng(feature.geometry.coordinates[1], feature.geometry.coordinates[0]);
                map.setView(latlng, 15);
                layer.openPopup();

                var linkContainer = document.getElementById('station-link-' + feature.properties.id);
                if (linkContainer.style.display === 'none' || linkContainer.style.display === '') {
                    linkContainer.style.display = 'block';
                    if (feature.properties.id === 'chk1') {
                        linkContainer.innerHTML = '<a href="https://www.forest.go.th/research-seed/" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (ศูนย์วนวัฒนวิจัยที่1 เชียงใหม่)</a>';
                    } else if (feature.properties.id === 'chk2') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (ศูนย์วนวัฒนวิจัยที่2 ลำปาง)</a>';
					} else if (feature.properties.id === 'chk3') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (ศูนย์วนวัฒนวิจัยที่3 กำแพงเพชร)</a>';
					} else if (feature.properties.id === 'chk4') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (ศูนย์วนวัฒนวิจัยที่4 กาญจนบุรี)</a>';
					} else if (feature.properties.id === 'chk5') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (ศูนย์วนวัฒนวิจัยที่5 ขอนแก่น)</a>';
					} else if (feature.properties.id === 'chk6') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (ศูนย์วนวัฒนวิจัยที่6 นครราชสีมา)</a>';
					} else if (feature.properties.id === 'chk7') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (ศูนย์วนวัฒนวิจัยที่7 ประจวบคีรีขันธ์)</a>';
					} else if (feature.properties.id === 'chk8') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (ศูนย์วนวัฒนวิจัยที่8 สุราษฎร์ธานี)</a>';
					} else if (feature.properties.id === 'chk9') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (ศูนย์วนวัฒนวิจัยที่9 สงขลา)</a>';
					} else if (feature.properties.id === 'chk10') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (ศูนย์เมล็ดพันธุ์ไม้ป่าภาคกลาง(สระบุรี))</a>';
					} else if (feature.properties.id === 'chk11') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (ศูนย์เมล็ดพันธุ์ไม้ป่าภาคตะวันออกเฉียงเหนือ(ขอนแก่น))</a>';
					} else if (feature.properties.id === 'chk12') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (ศูนย์เมล็ดพันธุ์ไม้ป่าภาคใต้(สงขลา))</a>';
					} else if (feature.properties.id === 'chk13') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (ศูนย์เมล็ดพันธุ์ไม้ป่าภาคเหนือ(ลำปาง))</a>';
					} else if (feature.properties.id === 'chk14') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยทรายทอง)</a>';
					} else if (feature.properties.id === 'chk15') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยทองผาภูมิ)</a>';
					} else if (feature.properties.id === 'chk16') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยท่าตูม)</a>';
					} else if (feature.properties.id === 'chk17') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยบ่อแก้ว)</a>';
					} else if (feature.properties.id === 'chk18') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยพิษณุโลก)</a>';
					} else if (feature.properties.id === 'chk19') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยแม่กา)</a>';
					} else if (feature.properties.id === 'chk20') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยแม่สะนาม)</a>';
					} else if (feature.properties.id === 'chk21') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยราชบุรี)</a>';
					} else if (feature.properties.id === 'chk22') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยลำเภา-ลำทราย)</a>';
					} else if (feature.properties.id === 'chk23') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยหนองคู)</a>';
					} else if (feature.properties.id === 'chk24') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยหมูสี)</a>';
					} else if (feature.properties.id === 'chk25') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยห้วยทา)</a>';
					} else if (feature.properties.id === 'chk26') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยห้วยบง)</a>';
					} else if (feature.properties.id === 'chk27') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยหินลับ)</a>';
					} else if (feature.properties.id === 'chk28') {
                        linkContainer.innerHTML = '<a href="https://forprod.forest.go.th/forprod/silvic/for_plant/index.html" target="_blank">คลิกที่นี่เพื่อเข้าชมเว็บไซต์ (สถานีวนวัฒนวิจัยอินทขิล)</a>';
                    }
                } else {
                    linkContainer.style.display = 'none';
                }

                var treeInfoContainer = document.getElementById("tree-info-container-" + feature.properties.id);
                treeInfoContainer.style.display = (treeInfoContainer.style.display === 'block' ? 'none' : 'block');
            });

            div.appendChild(checkbox);
            div.appendChild(spanText);
            checkboxForm.appendChild(div);

            var linkDiv = document.createElement("div");
            linkDiv.id = "station-link-" + feature.properties.id;
            linkDiv.className = "link-container";
            checkboxForm.appendChild(linkDiv);

            // เพิ่ม Popup พร้อมชื่อสถานี
            var popupContent = "<strong>" + feature.properties.name + "</strong><br>" + feature.properties.description;
            layer.bindPopup(popupContent);

            featureLayers[feature.properties.id] = layer;

            // กล่องข้อมูลพรรณไม้แยกกัน
			var treeInfoDiv = document.createElement("div");
			treeInfoDiv.id = "tree-info-container-" + feature.properties.id;
			treeInfoDiv.className = "tree-info-container";


            // เพิ่มข้อมูลพรรณไม้แยกเป็นกล่อง
			if (Array.isArray(feature.properties.treeInfo)) {
				feature.properties.treeInfo.forEach(function (info, index) {
					var treeBox = document.createElement("div");
					treeBox.className = "tree-info-box";
					treeBox.style.background = index % 2 === 0 ? "#e3f2fd" : "#dff0d8"; // สลับสีให้ดูดีขึ้น
					treeBox.style.padding = "10px";
					treeBox.style.borderRadius = "5px";
					treeBox.style.marginBottom = "5px";
					treeBox.style.boxShadow = "0 2px 5px rgba(0, 0, 0, 0.1)";
					treeBox.innerHTML = info;
					treeInfoDiv.appendChild(treeBox);
				});
			}
			checkboxForm.appendChild(treeInfoDiv);
        }

        L.geoJSON(geojsonFeatures, {
            onEachFeature: function (feature, layer) {
                addCheckbox(feature, layer);
            }
        }).addTo(map);

        function handleSearch(event) {
            if (event.key === "Enter") {
                searchStation();
            }
        }

        function searchStation() {
            var searchQuery = document.getElementById('search-input').value.toLowerCase();
            var found = false;

            for (var id in featureLayers) {
                var layer = featureLayers[id];
                var name = layer.feature.properties.name.toLowerCase();

                if (name.includes(searchQuery)) {
                    var latlng = L.latLng(layer.feature.geometry.coordinates[1], layer.feature.geometry.coordinates[0]);
                    map.setView(latlng, 15); // ซูมไปที่หมุด
                    layer.openPopup(); // เปิด Popup
                    found = true;
                    break;
                }
            }

            if (!found) {
                alert('ไม่พบสถานีที่ค้นหา');
            }
        }
    </script>
</body>
</html>
