add_subdirectory(PhysicsLists)

include_directories($ENV{GEANT4_FQ_DIR}/include)
include_directories($ENV{XERCES_C_INC})

art_make(
  MODULE_LIBRARIES
    art::Utilities
    cetlib_except::cetlib_except
    ROOT::Core
    ROOT::Hist
    ROOT::Physics
    ROOT::Geom
    ROOT::MathCore
    CLHEP::CLHEP
    Geant4::G4digits_hits
    Geant4::G4event
    Geant4::G4geometry
    Geant4::G4global
    Geant4::G4graphics_reps
    Geant4::G4materials
    Geant4::G4intercoms
    Geant4::G4particles
    Geant4::G4physicslists
    Geant4::G4processes
    Geant4::G4track
    Geant4::G4run
    sbndcode_LArG4_PhysicsLists

  LIB_LIBRARIES
    art::Utilities
    cetlib_except::cetlib_except
    ROOT::Core
    ROOT::Hist
    ROOT::Physics
    ROOT::Geom
    ROOT::MathCore
    CLHEP::CLHEP
    Geant4::G4digits_hits
    Geant4::G4event
    Geant4::G4geometry
    Geant4::G4global
    Geant4::G4graphics_reps
    Geant4::G4materials
    Geant4::G4intercoms
    Geant4::G4particles
    Geant4::G4physicslists
    Geant4::G4processes
    Geant4::G4track
    Geant4::G4run
    sbndcode_LArG4_PhysicsLists

  SERVICE_LIBRARIES
    art::Framework_Core
)

install_headers()
install_source()
install_fhicl()

