<!--TIMELINE??-->

<template>
  <div class="kt-portlet">
    <div>
      <b-navbar toggleable="lg" type="dark" variant="light">
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-nav-item-dropdown text="Démarches" right>
              <!--begin::Nav-->
              <ul class="kt-nav">
                <li class="kt-nav__head">
                  <img
                    svg-inline
                    class="kt-svg-icon--sm"
                    src="@/assets/media/flags/195-france.svg"
                    alt=""
                  />
                  
                  SIV
                  
                  <i
                    class="flaticon2-information"
                    v-b-tooltip.hover.bottom="'Les démarches auprès du Système d\'Immatriculation de Véhicules'"
                  ></i>
                </li>
                <li class="kt-nav__separator"></li>
                <li class="kt-nav__item">
                  <a href="#" class="kt-nav__link">
                    <i class="kt-nav__link-icon flaticon2-drop"></i>
                    <span class="kt-nav__link-text">DA/DAD</span>
                  </a>
                </li>
                <li class="kt-nav__item">
                  <a href="#" class="kt-nav__link">
                    <i class="kt-nav__link-icon flaticon2-calendar-8"></i>
                    <span class="kt-nav__link-text">DID</span>
                  </a>
                </li>
                <li class="kt-nav__item">
                  <a href="#" class="kt-nav__link">
                    <i class="kt-nav__link-icon flaticon2-telegram-logo"></i>
                    <span class="kt-nav__link-text">Déclaration de Cession</span>
                  </a>
                </li>
                <li class="kt-nav__item">
                  <a href="#" class="kt-nav__link">
                    <i class="kt-nav__link-icon flaticon2-new-email"></i>
                    <span class="kt-nav__link-text">Déclaration de Vente</span>
                    <span class="kt-nav__link-badge">
                      <span class="kt-badge kt-badge--success">5</span>
                    </span>
                  </a>
                </li>
                <li class="kt-nav__separator"></li>
                <li class="kt-nav__foot">
                  <a class="btn btn-label-brand btn-bold btn-sm" href="#"
                    >Upgrade plan</a
                  >
                  <a
                    class="btn btn-clean btn-bold btn-sm"
                    href="#"
                    v-b-tooltip.hover.bottom="'Click to learn more...'"
                    >Learn more</a
                  >
                </li>
              </ul>
              <!--end::Nav-->
            </b-nav-item-dropdown>

            <b-nav-item-dropdown right>
              <!-- Using 'button-content' slot -->
              <template v-slot:button-content>
                SIV
              </template>
              <b-dropdown-item href="#">

                
                    <i class="kt-nav__link-icon flaticon2-drop"></i>
                    <span class="kt-nav__link-text">DA/DAD sfsdf sdfsdfsd Poosd</span>
                  
              </b-dropdown-item>
              <b-dropdown-item href="#">Sign Out</b-dropdown-item>
            </b-nav-item-dropdown>
            <b-nav-form>
              <button
                v-on:click="submit"
                size="sm"
                class="btn btn-success btn-sm kt-font-bold kt-font-transform-u"
                data-ktwizard-type="action-submit"
              >
                Sauvegarder
              </button>
            </b-nav-form>

            <div
            class="dropdown dropdown-inline"
            v-b-tooltip.hover.left="'Quick actions'"
          >
            <a
              href="#"
              class="btn btn-icon"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="true"
            >
              <img
                svg-inline
                class="kt-svg-icon kt-svg-icon--success kt-svg-icon--md"
                src="@/assets/media/icons/svg/Files/File-plus.svg"
                alt=""
              />
              <!--<i class="flaticon2-plus"></i>-->
            </a>
            <div
              class="dropdown-menu dropdown-menu-lg dropdown-menu-left"
            >
              <!--begin::Nav-->
              <ul class="kt-nav">
                <li class="kt-nav__head">
                  Add anything or jump to:
                  <i
                    class="flaticon2-information"
                    v-b-tooltip.hover.bottom="'Click to learn more...'"
                  ></i>
                </li>
                <li class="kt-nav__separator"></li>
                <li class="kt-nav__item">
                  <a href="#" class="kt-nav__link">
                    <i class="kt-nav__link-icon flaticon2-drop"></i>
                    <span class="kt-nav__link-text">Order</span>
                  </a>
                </li>
                <li class="kt-nav__item">
                  <a href="#" class="kt-nav__link">
                    <i class="kt-nav__link-icon flaticon2-calendar-8"></i>
                    <span class="kt-nav__link-text">Ticket</span>
                  </a>
                </li>
                <li class="kt-nav__item">
                  <a href="#" class="kt-nav__link">
                    <i class="kt-nav__link-icon flaticon2-telegram-logo"></i>
                    <span class="kt-nav__link-text">Goal</span>
                  </a>
                </li>
                <li class="kt-nav__item">
                  <a href="#" class="kt-nav__link">
                    <i class="kt-nav__link-icon flaticon2-new-email"></i>
                    <span class="kt-nav__link-text">Support Case</span>
                    <span class="kt-nav__link-badge">
                      <span class="kt-badge kt-badge--success">5</span>
                    </span>
                  </a>
                </li>
                <li class="kt-nav__separator"></li>
                <li class="kt-nav__foot">
                  <a class="btn btn-label-brand btn-bold btn-sm" href="#"
                    >Upgrade plan</a
                  >
                  <a
                    class="btn btn-clean btn-bold btn-sm"
                    href="#"
                    v-b-tooltip.hover.bottom="'Click to learn more...'"
                    >Learn more</a
                  >
                </li>
              </ul>
              <!--end::Nav-->
            </div>
          </div>

          </b-navbar-nav>
        
      </b-navbar>
    </div>
    <div class="kt-portlet__body kt-portlet__body--fit">      
      <div
        class="kt-grid kt-wizard-v2 kt-wizard-v2--white"
        id="kt_wizard_v2"
        data-ktwizard-state="step-first"
      >
        <div class="kt-grid__item kt-wizard-v2__aside">
          <!--begin: Form Wizard Nav -->
          <div class="kt-wizard-v2__nav">
            <div
              class="kt-wizard-v2__nav-items kt-wizard-v2__nav-items--clickable"
            >
              <!--doc: Replace A tag with SPAN tag to disable the step link click -->
              <div
                class="kt-wizard-v2__nav-item"
                data-ktwizard-type="step"
                data-ktwizard-state="current"
              >
                <div class="kt-wizard-v2__nav-body">
                  <div class="kt-wizard-v2__nav-icon">
                    <i class="flaticon-globe"></i>
                  </div>
                  <div class="kt-wizard-v2__nav-label">
                    <div class="kt-wizard-v2__nav-label-title">
                      Véhicule
                    </div>
                    <div class="kt-wizard-v2__nav-label-desc">
                      Informations Techniques et Certificat d'Immatriculation
                    </div>
                  </div>
                </div>
              </div>
              <div class="kt-wizard-v2__nav-item" data-ktwizard-type="step">
                <div class="kt-wizard-v2__nav-body">
                  <div class="kt-wizard-v2__nav-icon">
                    <i class="flaticon-bus-stop"></i>
                  </div>
                  <div class="kt-wizard-v2__nav-label">
                    <div class="kt-wizard-v2__nav-label-title">Provenance</div>
                    <div class="kt-wizard-v2__nav-label-desc">
                      Infos Vendeurs Fournisseurs Transporteurs
                    </div>
                  </div>
                </div>
              </div>
              <div
                class="kt-wizard-v2__nav-item"
                href="#"
                data-ktwizard-type="step"
              >
                <div class="kt-wizard-v2__nav-body">
                  <div class="kt-wizard-v2__nav-icon">
                    <i class="flaticon-responsive"></i>
                  </div>
                  <div class="kt-wizard-v2__nav-label">
                    <div class="kt-wizard-v2__nav-label-title">Dossier</div>
                    <div class="kt-wizard-v2__nav-label-desc">
                      Informations et Statut du Dossiers
                    </div>
                  </div>
                </div>
              </div>
              <div class="kt-wizard-v2__nav-item" data-ktwizard-type="step">
                <div class="kt-wizard-v2__nav-body">
                  <div class="kt-wizard-v2__nav-icon">
                    <i class="flaticon-trophy"></i>
                  </div>
                  <div class="kt-wizard-v2__nav-label">
                    <div class="kt-wizard-v2__nav-label-title">Etat</div>
                    <div class="kt-wizard-v2__nav-label-desc">
                      Informations, Descriptifs et Photos du Véhicule
                    </div>
                  </div>
                </div>
              </div>
              <div class="kt-wizard-v2__nav-item" data-ktwizard-type="step">
                <div class="kt-wizard-v2__nav-body">
                  <div class="kt-wizard-v2__nav-icon">
                    <i class="flaticon-truck"></i>
                  </div>
                  <div class="kt-wizard-v2__nav-label">
                    <div class="kt-wizard-v2__nav-label-title">Documents</div>
                    <div class="kt-wizard-v2__nav-label-desc">
                      Différents Documents Relatif au Véhicule
                    </div>
                  </div>
                </div>
              </div>
              <div class="kt-wizard-v2__nav-item" data-ktwizard-type="step">
                <div class="kt-wizard-v2__nav-body">
                  <div class="kt-wizard-v2__nav-icon">
                    <i class="flaticon-confetti"></i>
                  </div>
                  <div class="kt-wizard-v2__nav-label">
                    <div class="kt-wizard-v2__nav-label-title">Financier</div>
                    <div class="kt-wizard-v2__nav-label-desc">
                      Informations Financières
                    </div>
                  </div>
                </div>
              </div>
              <div class="kt-wizard-v2__nav-item" data-ktwizard-type="step">
                <div class="kt-wizard-v2__nav-body">
                  <div class="kt-wizard-v2__nav-icon">
                    <i class="flaticon-confetti"></i>
                  </div>
                  <div class="kt-wizard-v2__nav-label">
                    <div class="kt-wizard-v2__nav-label-title">Validation</div>
                    <div class="kt-wizard-v2__nav-label-desc">Validation</div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!--end: Form Wizard Nav -->
        </div>
        <div class="kt-grid__item kt-grid__item--fluid kt-wizard-v2__wrapper">

          <!--begin: Form Wizard Form-->
          <form class="kt-form" id="kt_form">
            <!--begin: Form Wizard Step 1-->
            <div
              class="kt-wizard-v2__content"
              data-ktwizard-type="step-content"
              data-ktwizard-state="current"
            >
              <div class="kt-form__section kt-form__section--first">
                <div class="kt-wizard-v2__form">
                  <div class="row">
                    <b-media right-align vertical-align="center">
                      <template v-slot:aside>
                        <b-img
                          blank
                          blank-color="#ccc"
                          width="100"
                          alt="placeholder"
                        ></b-img>
                      </template>
                    </b-media>
                    <div class="col-xl-3 col-lg-3 col-md-8 col-sm-8 col-12">
                      <div class="form-group">
                        <label>Immatriculation</label>
                        <b-input-group>
                          <b-input-group-prepend is-text>
                            <b-form-checkbox
                              switch
                              class="mr-n2"
                              name="second_reg_number"
                            >
                              <span class="sr-only"
                                >Deuxième Immatriculation</span
                              >
                            </b-form-checkbox>
                          </b-input-group-prepend>
                          <b-form-input
                            aria-label="Immatriculation"
                            id="reg_number"
                            name="reg_number"
                          ></b-form-input>
                          <b-input-group-append>
                            <b-button variant="outline-secondary"
                              ><i class="fas fa-search"></i
                            ></b-button>
                          </b-input-group-append>
                        </b-input-group>
                        <span class="form-text text-muted">Immatriculation (A). Cocher si 2ème Immat</span>
                      </div>
                    </div>

                    <!--Deuxième immatriculation si checkbox vrai-->

                    <div
                      hidden
                      class="col-xl-3 col-lg-3 col-md-8 col-sm-8 col-12"
                      id="2nd_reg_number"
                    >
                      <div class="form-group">
                        <label>2ème Immat.</label>
                        <b-input-group>
                          <b-form-input
                            aria-label="Immatriculation"
                            id="2nd_reg_number"
                            name="snd_reg_number"
                          ></b-form-input>
                        </b-input-group>
                        <span class="form-text text-muted">2ème Immat Disponible (A.1)</span>
                      </div>
                    </div>

                    <div class="col-xl-3 col-lg-3 col-md-6 col-sm-6 col-12">
                      <div class="form-group">
                        <label>Num. de Série (VIN)</label>
                        <b-input-group>
                          <b-form-input
                            aria-label="serial_number"
                          ></b-form-input>
                          <b-input-group-append>
                            <b-button variant="outline-secondary"
                              ><i class="fa fa-search"></i
                            ></b-button>
                          </b-input-group-append>
                        </b-input-group>
                        <span class="form-text text-muted">Num. d'Identification du Véhicule (E)	</span>
                      </div>
                    </div>
                    <div class="col-xl-3 col-lg-3 col-md-6 col-sm-6 col-12">
                      <div class="form-group">
                        <label>Numéro CNIT</label>
                        <b-input-group>
                          <b-form-input
                            aria-label="cnit_type_mine"
                          ></b-form-input>
                          
                        </b-input-group>
                        <span class="form-text text-muted">Type Mine (D.2.1)</span>
                      </div>                      
                    </div>
                  </div>

                  <div>
                    <b-card no-body>
                    <b-tabs v-model="tabIndex" align="right" small card pills>
                      <b-tab title="Véhicule" active>
                        <div class="form-group row">
                          <div
                            class="col-xl-2 col-lg-3 col-md-6 col-sm-6 col-12"
                          >
                            <label>Marque</label>
                            <select
                              class="form-control kt-select2"
                              id="kt_select2_1"
                              name="eolv_make"
                            >
                              <option></option>
                              <option value="RENAULT">Renault</option>
                              <option value="PEUGEOT">Peugeot</option>
                              <option value="CITROEN">Citroën</option>
                              <option value="VOLKSWAGEN">Volkswagen</option>
                              <option value="Toyota">Toyota</option>
                              <option value="Opel">Opel</option>
                              <option value="Fiat">Fiat</option>
                              <option value="Mercedes">Mercedes</option>
                              <option value="Seat">Seat</option>
                            </select>
                            <span class="form-text text-muted">Marque Véhicule (D.1)</span>
                          </div>
                          <div
                            class="col-xl-2 col-lg-3 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Gamme</label>
                              <div class="kt-input-icon kt-input-icon--right">
                                <input
                                  type="text"
                                  class="form-control"
                                  name="gamme"
                                  placeholder=""
                                  value
                                />
                              </div>
                              <span class="form-text text-muted">Gamme Véhicule (D.2)</span>
                            </div>
                          </div>
                          <div
                            class="col-xl-2 col-lg-3 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Modèle</label>
                              <input
                                type="text"
                                class="form-control"
                                name="modele"
                                placeholder=""
                                value
                              />
                              <span class="form-text text-muted">Modèle Véhicule (D.3)</span>
                            </div>
                          </div>
                          <div
                            class="col-xl-2 col-lg-3 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Version</label>
                              <input
                                type="text"
                                class="form-control"
                                name="version"
                                placeholder=""
                                value
                              />
                              <span class="form-text text-muted">Version Véhicule</span>
                            </div>
                          </div>
                          <div
                            class="col-xl-2 col-lg-3 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Finition</label>
                              <input
                                type="text"
                                class="form-control"
                                name="finition"
                                placeholder=""
                                value
                              />
                              <span class="form-text text-muted">Finition Véhicule</span>
                            </div>
                          </div>
                          
                          <div
                            class="col-xl-2 col-lg-3 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Carburant</label>
                              <input
                                type="text"
                                class="form-control"
                                name="couleur"
                                placeholder=""
                                value
                              />
                              <span class="form-text text-muted">Carburant (P.3)</span>
                            </div>
                          </div>
                          <div
                            class="col-xl-2 col-lg-3 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Couleur</label>
                              <input
                                type="text"
                                class="form-control"
                                name="couleur"
                                placeholder=""
                                value
                              />
                              <span class="form-text text-muted">Couleur Réelle</span>
                            </div>
                          </div>

                          <div
                            class="col-xl-2 col-lg-3 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Code Coul</label>
                              <input
                                type="text"
                                class="form-control"
                                name="codecouleur"
                                placeholder=""
                                value
                              />
                              <span class="form-text text-muted">Code Couleur</span>
                            </div>
                          </div>
                          <div
                            class="col-xl-2 col-lg-3 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Nb Portes</label>
                              <select
                                class="form-control kt-select2"
                                id="kt_select2_3"
                                name="nbrportes"
                              >
                                <option></option>
                                <option value="5P">5</option>
                                <option value="3P">3</option>
                                <option value="CoffreBat">Autre</option>
                              </select>
                              <span class="form-text text-muted">Nombre de Portes</span>
                            </div>
                          </div>
                          <div
                            class="col-xl-2 col-lg-2 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Coffre</label>
                              <select
                                class="form-control kt-select2"
                                id="kt_select2_4"
                                name="typecoffre"
                              >
                                <option></option>
                                <option value="CoffreHay">Hayon</option>
                                <option value="CoffreBat">Battant</option>
                                <option value="CoffreBat">Autre</option>
                              </select>
                              <span class="form-text text-muted">Type de Coffre</span>
                            </div>
                          </div>
                          <div
                            class="col-xl-2 col-lg-2 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Cyl</label>
                              <input
                                type="text"
                                class="form-control"
                                name="modele"
                                placeholder=""
                                value
                              />
                              <span class="form-text text-muted">Cylindrés en cm3</span>
                            </div>
                          </div>
                          <div
                            class="col-xl-2 col-lg-2 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Puissance</label>
                              <input
                                type="text"
                                class="form-control"
                                name="power"
                                placeholder=""
                                value
                              />
                              <span class="form-text text-muted">Nombre de Chevaux</span>
                            </div>
                          </div>
                          <div
                            class="col-xl-2 col-lg-2 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Fisc.</label>
                              <input
                                type="text"
                                class="form-control"
                                name="finition"
                                placeholder=""
                                value
                              />
                              <span class="form-text text-muted">Chevaux Fiscaux (P.6)</span>
                            </div>
                          </div>
                          <div
                            class="col-xl-2 col-lg-3 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Code Moteur</label>
                              <input
                                type="text"
                                class="form-control"
                                name="codemoteur"
                                placeholder=""
                                value
                              />
                              <span class="form-text text-muted">Code Moteur</span>
                            </div>
                          </div>
                          <div
                            class="col-xl-2 col-lg-3 col-md-6 col-sm-6 col-12"
                          >
                            <div class="form-group">
                              <label>Code Boite</label>
                              <input
                                type="text"
                                class="form-control"
                                name="codeboite"
                                placeholder=""
                                value
                              />
                              <span class="form-text text-muted">Code Boite</span>
                            </div>
                          </div>
                          <div class="col-xl-2 col-lg-2 col-md-6 col-sm-6 col-12">
                            <div class="form-group">
                              <label>Type</label>
                              <select
                                class="form-control kt-select2"
                                id="kt_select2_5"
                                name="typeboite"
                              >
                                <option></option>
                                <option value="Manuelle">Manuelle</option>
                                <option value="Automatique">Automatique</option>
                                <option value="SemiAuto">Semi Auto.</option>
                              </select>
                              <span class="form-text text-muted">Type de Transmission</span>
                            </div>                         
                          </div>
                        </div>
                      </b-tab>
                      <b-tab title="Certificat Immatriculation">
                        <!--begin: Certificat d Immatriculation-->
                        <div class="form-group row">
                          <div
                            class="col-xl-3 col-lg-3 col-md-6 col-sm-6 col-12"
                          >
                            <label>1ère Immatriculation</label>
                            <div class="input-group">
                              <input
                                type="text"
                                class="form-control"
                                name="date"
                                placeholder="Select date"
                                id="kt_datepicker"
                              />
                              <div class="input-group-append">
                                <span class="input-group-text">
                                  <i class="la la-calendar-check-o"></i>
                                </span>
                              </div>
                            </div>
                            <span class="form-text text-muted">Date de 1ère Immatriculation (B)</span>
                          </div>
                          <div class="col-xl-3 col-lg-3 col-md-6 col-sm-6 col-12">
                            <div class="form-group">
                              <label>Nom du Titulaire</label>
                              <input
                                type="text"
                                class="form-control"
                                name="nomtitulaire"
                                placeholder=""
                                value=""
                              />
                              <span class="form-text text-muted">Nom du Titulaire (C.1)</span>  
                            </div>
                          </div>
                          <div class="col-xl-3 col-lg-3 col-md-6 col-sm-6 col-12">
                            <div class="form-group">
                              <label>Prénom</label>
                              <input
                                type="text"
                                class="form-control"
                                name="prenomtitulaire"
                                placeholder=""
                                value=""
                              />
                              <span class="form-text text-muted">Prénom (C.1)</span>  
                            </div>
                          </div>
                      <div class="col-xl-3 col-lg-3 col-md-6 col-sm-6 col-12">
                      <div class="form-group">
                        <label>Autre Titulaire</label>
                        <b-input-group>
                          <b-input-group-prepend is-text>
                            <b-form-checkbox
                              switch
                              class="mr-n2"
                              name="second_reg_number" >
                              <span class="sr-only">Deuxième Immatriculation</span>
                            </b-form-checkbox>
                          </b-input-group-prepend>
                          <b-form-input aria-label="Immatriculation" id="reg_number" name="reg_number"></b-form-input>
                        </b-input-group>
                        <span class="form-text text-muted">Est Propriétaire (C.4.a) (C.4.1)</span>
                      </div>
                    </div>
                          <div class="col-xl-5 col-lg-5 col-md-6 col-sm-6 col-12">
                            <div class="form-group">
                              <label>Adresse</label>
                              <input
                                type="text"
                                class="form-control"
                                name="nomtitulaire"
                                placeholder=""
                                value=""
                              />
                              <span class="form-text text-muted">Adresse (C.3)</span>  
                            </div>
                          </div>
                          <div class="col-xl-2 col-lg-2 col-md-6 col-sm-6 col-12">
                            <div class="form-group">
                              <label>CP.</label>
                              <input
                                type="text"
                                class="form-control"
                                name="prenomtitulaire"
                                placeholder=""
                                value=""
                              />
                              <span class="form-text text-muted">Code Postal (C.3)</span>  
                            </div>
                          </div>
                          <div class="col-xl-2 col-lg-2 col-md-6 col-sm-6 col-12">
                            <div class="form-group">
                              <label>Ville</label>
                              <input
                                type="text"
                                class="form-control"
                                name="prenomtitulaire"
                                placeholder=""
                                value=""
                              />
                              <span class="form-text text-muted">Commune (C.3)</span>  
                            </div>
                          </div>
                        </div>

                        <div class="form-group row">                      
                          <div class="col-xl-3 col-lg-3 col-md-6 col-sm-6 col-12">
                            <label>Date Certificat</label>
                            <div class="input-group">
                              <input
                                type="text"
                                class="form-control"
                                name="date"
                                placeholder="Select date"
                                id="kt_datepicker"
                              />
                              <div class="input-group-append">
                                <span class="input-group-text">
                                  <i class="la la-calendar-check-o"></i>
                                </span>
                              </div>                            
                            </div>
                            <span class="form-text text-muted">Date du Certificat (I)</span> 
                          </div>
                          


                          <!--CACHER NUMERO DE FORMULE SI ANCIENNE IMMAT-->
                          <div class="col-xl-2 col-lg-2 col-md-6 col-sm-6 col-12">
                            <div class="form-group">
                              <label>Num. Formule</label>
                              <input
                                type="text"
                                class="form-control"
                                name="version"
                                placeholder=""
                                value
                              />
                              <span class="form-text text-muted">Formule de CI</span>
                            </div>
                          </div>
                          <div class="col-xl-2 col-lg-3 col-md-6 col-sm-6 col-12">
                            <div class="form-group">
                              <label>Genre</label>
                              <select
                                class="form-control kt-select2"
                                id="kt_select2_2"
                                name="genre"
                              >
                                <option></option>
                                <option value="VP">VP</option>
                                <option value="VL">VL</option>
                                <option value="Autregenre">Autre</option>
                              </select>
                              <span class="form-text text-muted">Genre National (J.1)</span>
                            </div>
                          </div>
                          <div class="col-xl-2 col-lg-2 col-md-6 col-sm-6 col-12">
                            <div class="form-group">
                              <label>Poids à Vide</label>
                              <input
                                type="text"
                                class="form-control"
                                name="poidsavide"
                                placeholder=""
                                value=""
                              />
                              <span class="form-text text-muted">Poids à Vide (G.1)</span>  
                            </div>
                          </div>
                        </div>
                        <div>
                          <!-- Using modifiers -->
                          <b-button v-b-toggle.collapse-1 class="m-1">Autres Champs</b-button>

                          <!-- Element to collapse -->
                          <b-collapse id="collapse-1">
                            <b-card>
                              <div class="col-xl-2 col-lg-2 col-md-6 col-sm-6 col-12">
                                <div class="form-group">
                                  <label>Poids à Vide</label>
                                  <input
                                    type="text"
                                    class="form-control"
                                    name="poidsavide"
                                    placeholder=""
                                    value=""
                                  />
                                  <span class="form-text text-muted">Poids à Vide (G.1)</span>  
                                </div>
                              </div>
                              <div class="col-xl-2 col-lg-2 col-md-6 col-sm-6 col-12">
                                <div class="form-group">
                                  <label>Poids Total</label>
                                  <input
                                    type="text"
                                    class="form-control"
                                    name="poidsavide"
                                    placeholder=""
                                    value=""
                                  />
                                  <span class="form-text text-muted">Poids Total (G.2)</span>  
                                </div>
                              </div>


                            </b-card>
                          </b-collapse>
                        </div>

                        <!--end: Certificat d Immatriculation-->
                      </b-tab>
                      <b-tab title="Etat d'Entrée">
                        <p>I'm a disabled tab!</p>
                      </b-tab>
                    </b-tabs>
                    </b-card>
                  </div>
                </div>
              </div>
            </div>
            <!--end: Form Wizard Step 1-->

            <!--begin: Form Wizard Step 2-->
            <div class="kt-wizard-v2__content" data-ktwizard-type="step-content">

              <div class="kt-form__section kt-form__section--first">
                <b-card no-body>
                    <b-tabs v-model="tabIndex" align="right" small card>
                      <b-tab title="Vendeur - Fournisseur" active>

                      </b-tab>
                      <b-tab title="Propriétaire">

                      </b-tab>
                      <b-tab title="Dépositaire">

                      </b-tab>
                      <b-tab title="Transporteur">

                      </b-tab>
                    </b-tabs>
                </b-card>
                
                
                
                <div class="kt-wizard-v2__form">
                  <div class="row">
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>Address Line 1</label>
                        <input
                          type="text"
                          class="form-control"
                          name="address1"
                          placeholder="Address Line 1"
                          value="Address Line 1"
                        />
                        <span class="form-text text-muted">Please enter your Address.</span
                        >
                      </div>
                    </div>
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>Address Line 2</label>
                        <input
                          type="text"
                          class="form-control"
                          name="address2"
                          placeholder="Address Line 2"
                          value="Address Line 2"
                        />
                        <span class="form-text text-muted"
                          >Please enter your Address.</span
                        >
                      </div>
                    </div>
                  </div>
                  <div class="row">
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>Postcode</label>
                        <input
                          type="text"
                          class="form-control"
                          name="postcode"
                          placeholder="Postcode"
                          value="3000"
                        />
                        <span class="form-text text-muted"
                          >Please enter your Postcode.</span
                        >
                      </div>
                    </div>
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>City</label>
                        <input
                          type="text"
                          class="form-control"
                          name="city"
                          placeholder="City"
                          value="Melbourne"
                        />
                        <span class="form-text text-muted"
                          >Please enter your City.</span
                        >
                      </div>
                    </div>
                  </div>
                  <div class="row">
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>State</label>
                        <input
                          type="text"
                          class="form-control"
                          name="state"
                          placeholder="State"
                          value="VIC"
                        />
                        <span class="form-text text-muted"
                          >Please enter your Postcode.</span
                        >
                      </div>
                    </div>
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>Country:</label>
                        <select name="country" class="form-control">
                          <option value>Select</option>
                          <option value="AF">Afghanistan</option>
                          <option value="AX">Åland Islands</option>
                          <option value="AL">Albania</option>
                          <option value="AU" selected>Australia</option>
                        </select>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <!--end: Form Wizard Step 2-->

            <!--begin: Form Wizard Step 3-->
            <div
              class="kt-wizard-v2__content"
              data-ktwizard-type="step-content"
            >
              <div class="kt-heading kt-heading--md">Select your Services</div>
              <div class="kt-form__section kt-form__section--first">
                <div class="kt-wizard-v2__form">
                  <div class="form-group">
                    <label>Delivery Type</label>
                    <select name="delivery" class="form-control">
                      <option value>Select a Service Type Option</option>
                      <option value="overnight" selected
                        >Overnight Delivery (within 48 hours)</option
                      >
                      <option value="express"
                        >Express Delivery (within 5 working days)</option
                      >
                      <option value="basic"
                        >Basic Delivery (within 5 - 10 working days)</option
                      >
                    </select>
                  </div>
                  <div class="form-group">
                    <label>Packaging Type</label>
                    <select name="packaging" class="form-control">
                      <option value>Select a Packaging Type Option</option>
                      <option value="regular" selected
                        >Regular Packaging</option
                      >
                      <option value="oversized">Oversized Packaging</option>
                      <option value="fragile">Fragile Packaging</option>
                      <option value="frozen">Frozen Packaging</option>
                    </select>
                  </div>
                  <div class="form-group">
                    <label>Preferred Delivery Window</label>
                    <select name="preferreddelivery" class="form-control">
                      <option value>Select a Preferred Delivery Option</option>
                      <option value="morning" selected
                        >Morning Delivery (8:00AM - 11:00AM)</option
                      >
                      <option value="afternoon"
                        >Afternoon Delivery (11:00AM - 3:00PM)</option
                      >
                      <option value="evening"
                        >Evening Delivery (3:00PM - 7:00PM)</option
                      >
                    </select>
                  </div>
                </div>
              </div>
            </div>
            <!--end: Form Wizard Step 3-->

            <!--begin: Form Wizard Step 4-->
            <div
              class="kt-wizard-v2__content"
              data-ktwizard-type="step-content"
            >
              <div class="kt-heading kt-heading--md">
                Setup Your Delivery Location
              </div>
              <div class="kt-form__section kt-form__section--first">
                <div class="kt-wizard-v2__form">
                  <div class="row">
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>Address Line 1</label>
                        <input
                          type="text"
                          class="form-control"
                          name="locaddress1"
                          placeholder="Address Line 1"
                          value="Address Line 1"
                        />
                        <span class="form-text text-muted"
                          >Please enter your Address.</span
                        >
                      </div>
                    </div>
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>Address Line 2</label>
                        <input
                          type="text"
                          class="form-control"
                          name="locaddress2"
                          placeholder="Address Line 2"
                          value="Address Line 2"
                        />
                        <span class="form-text text-muted"
                          >Please enter your Address.</span
                        >
                      </div>
                    </div>
                  </div>
                  <div class="row">
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>Postcode</label>
                        <input
                          type="text"
                          class="form-control"
                          name="locpostcode"
                          placeholder="Postcode"
                          value="3072"
                        />
                        <span class="form-text text-muted"
                          >Please enter your Postcode.</span
                        >
                      </div>
                    </div>
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>City</label>
                        <input
                          type="text"
                          class="form-control"
                          name="loccity"
                          placeholder="City"
                          value="Preston"
                        />
                        <span class="form-text text-muted"
                          >Please enter your City.</span
                        >
                      </div>
                    </div>
                  </div>
                  <div class="row">
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>State</label>
                        <input
                          type="text"
                          class="form-control"
                          name="locstate"
                          placeholder="State"
                          value="VIC"
                        />
                        <span class="form-text text-muted"
                          >Please enter your Postcode.</span
                        >
                      </div>
                    </div>
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>Country:</label>
                        <select name="loccountry" class="form-control">
                          <option value>Select</option>
                          <option value="AF">Afghanistan</option>
                          <option value="AX">Åland Islands</option>
                          <option value="AL">Albania</option>
                          <option value="DZ">Algeria</option>
                          <option value="AS">American Samoa</option>
                          <option value="AD">Andorra</option>
                          <option value="AO">Angola</option>
                          <option value="AI">Anguilla</option>
                          <option value="AQ">Antarctica</option>
                          <option value="AG">Antigua and Barbuda</option>
                        </select>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <!--end: Form Wizard Step 4-->

            <!--begin: Form Wizard Step 5-->
            <div
              class="kt-wizard-v2__content"
              data-ktwizard-type="step-content"
            >
              <div class="kt-heading kt-heading--md">
                Enter your Payment Details
              </div>
              <div class="kt-form__section kt-form__section--first">
                <div class="kt-wizard-v2__form">
                  <div class="row">
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>Name on Card</label>
                        <input
                          type="text"
                          class="form-control"
                          name="ccname"
                          placeholder="Card Name"
                          value="John Wick"
                        />
                        <span class="form-text text-muted"
                          >Please enter your Card Name.</span
                        >
                      </div>
                    </div>
                    <div class="col-xl-6">
                      <div class="form-group">
                        <label>Card Number</label>
                        <input
                          type="text"
                          class="form-control"
                          name="ccnumber"
                          placeholder="Card Number"
                          value="4444 3333 2222 1111"
                        />
                        <span class="form-text text-muted"
                          >Please enter your Address.</span
                        >
                      </div>
                    </div>
                  </div>
                  <div class="row">
                    <div class="col-xl-4">
                      <div class="form-group">
                        <label>Card Expiry Month</label>
                        <input
                          type="number"
                          class="form-control"
                          name="ccmonth"
                          placeholder="Card Expiry Month"
                          value="01"
                        />
                        <span class="form-text text-muted"
                          >Please enter your Card Expiry Month.</span
                        >
                      </div>
                    </div>
                    <div class="col-xl-4">
                      <div class="form-group">
                        <label>Card Expiry Year</label>
                        <input
                          type="number"
                          class="form-control"
                          name="ccyear"
                          placeholder="Card Expire Year"
                          value="21"
                        />
                        <span class="form-text text-muted"
                          >Please enter your Card Expiry Year.</span
                        >
                      </div>
                    </div>
                    <div class="col-xl-4">
                      <div class="form-group">
                        <label>Card CVV Number</label>
                        <input
                          type="password"
                          class="form-control"
                          name="cccvv"
                          placeholder="Card CVV Number"
                          value="123"
                        />
                        <span class="form-text text-muted"
                          >Please enter your Card CVV Number.</span
                        >
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <!--end: Form Wizard Step 5-->

            <!--begin: Form Wizard Step 6-->
            <div
              class="kt-wizard-v2__content"
              data-ktwizard-type="step-content"
            >
              <div class="kt-heading kt-heading--md">
                Review your Details and Submit
              </div>
              <div class="kt-form__section kt-form__section--first">
                <div class="kt-wizard-v2__review">
                  <div class="kt-wizard-v2__review-item">
                    <div class="kt-wizard-v2__review-title">
                      Account Details
                    </div>
                    <div class="kt-wizard-v2__review-content">
                      John Wick
                      <br />Phone: +61412345678 <br />Email: johnwick@reeves.com
                    </div>
                  </div>
                  <div class="kt-wizard-v2__review-item">
                    <div class="kt-wizard-v2__review-title">
                      Support Location Address
                    </div>
                    <div class="kt-wizard-v2__review-content">
                      Address Line 1
                      <br />Address Line 2 <br />Melbourne 3000, VIC, Australia
                    </div>
                  </div>
                  <div class="kt-wizard-v2__review-item">
                    <div class="kt-wizard-v2__review-title">
                      Support Channels
                    </div>
                    <div class="kt-wizard-v2__review-content">
                      Overnight Delivery with Regular Packaging
                      <br />Preferred Morning (8:00AM - 11:00AM) Delivery
                    </div>
                  </div>
                  <div class="kt-wizard-v2__review-item">
                    <div class="kt-wizard-v2__review-title">
                      Delivery Address
                    </div>
                    <div class="kt-wizard-v2__review-content">
                      Address Line 1
                      <br />Address Line 2 <br />Preston 3072, VIC, Australia
                    </div>
                  </div>
                  <div class="kt-wizard-v2__review-item">
                    <div class="kt-wizard-v2__review-title">
                      Payment Details
                    </div>
                    <div class="kt-wizard-v2__review-content">
                      Card Number: xxxx xxxx xxxx 1111
                      <br />Card Name: John Wick <br />Card Expiry: 01/21
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <!--end: Form Wizard Step 6-->

            <div
              class="kt-wizard-v2__content"
              data-ktwizard-type="step-content"
            >
              <div class="kt-heading kt-heading--md">
                Review your Details and Submit
              </div>
              <div class="kt-form__section kt-form__section--first">
                <div class="kt-wizard-v2__review">
                  <div class="kt-wizard-v2__review-item">
                    <div class="kt-wizard-v2__review-title">
                      Account Details
                    </div>
                    <div class="kt-wizard-v2__review-content">
                      John Wick
                      <br />Phone: +61412345678 <br />Email: johnwick@reeves.com
                    </div>
                  </div>
                  <div class="kt-wizard-v2__review-item">
                    <div class="kt-wizard-v2__review-title">
                      Support Location Address
                    </div>
                    <div class="kt-wizard-v2__review-content">
                      Address Line 1
                      <br />Address Line 2 <br />Melbourne 3000, VIC, Australia
                    </div>
                  </div>
                  <div class="kt-wizard-v2__review-item">
                    <div class="kt-wizard-v2__review-title">
                      Support Channels
                    </div>
                    <div class="kt-wizard-v2__review-content">
                      Overnight Delivery with Regular Packaging
                      <br />Preferred Morning (8:00AM - 11:00AM) Delivery
                    </div>
                  </div>
                  <div class="kt-wizard-v2__review-item">
                    <div class="kt-wizard-v2__review-title">
                      Delivery Address
                    </div>
                    <div class="kt-wizard-v2__review-content">
                      Address Line 1
                      <br />Address Line 2 <br />Preston 3072, VIC, Australia
                    </div>
                  </div>
                  <div class="kt-wizard-v2__review-item">
                    <div class="kt-wizard-v2__review-title">
                      Payment Details
                    </div>
                    <div class="kt-wizard-v2__review-content">
                      Card Number: xxxx xxxx xxxx 1111
                      <br />Card Name: John Wick <br />Card Expiry: 01/21
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <!--end: Form Wizard Step 7-->

            <!--begin: Form Actions -->
            <div class="kt-form__actions">
              <button
                v-on:click="addvehicleverifycoherence"
                class="btn btn-secondary btn-md btn-tall btn-wide kt-font-bold kt-font-transform-u"
                data-ktwizard-type="action-prev"
              >
                Previous
              </button>
              <button
                v-on:click="submit"
                class="btn btn-success btn-md btn-tall btn-wide kt-font-bold kt-font-transform-u"
                data-ktwizard-type="action-submit"
              >
                Submit
              </button>
              <button
                v-on:click="addvehicleverifycoherence"
                class="btn btn-brand btn-md btn-tall btn-wide kt-font-bold kt-font-transform-u"
                data-ktwizard-type="action-next"
              >
                Next Step
              </button>
            </div>
            <!--end: Form Actions -->
          </form>
          <!--end: Form Wizard Form-->
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@import "@/assets/sass/pages/wizard/wizard-2.scss";
</style>

<script>
import { SET_BREADCRUMB } from "@/store/breadcrumbs.module";
import KTUtil from "@/assets/js/util";
import KTWizard from "@/assets/js/wizard";
import Swal from "sweetalert2";
//import KTPortlet from "@/views/partials/content/Portlet.vue";
//import ContextMenu1 from "@/views/partials/widgets/ContextMenu1.vue";

export default {
  name: "addvehicle",
  components: {
    //KTPortlet,
    //ContextMenu1
  },
  mounted() {
    this.$store.dispatch(SET_BREADCRUMB, [
      { title: "Gestion de Véhicules", route: "addvehicle" },
      { title: "Ajouter Véhicule" }
    ]);

    // Initialize form wizard
    const wizard = new KTWizard("kt_wizard_v2", {
      startStep: 1, // initial active step number
      clickableSteps: true // allow step clicking
    });

    // Validation before going to next page
    //wizard.on("beforeNext", function(/*wizardObj*/) {
    // validate the form and use below function to stop the wizard's step
    // wizardObj.stop();
    //});

    // Change event
    wizard.on("change", function(/*wizardObj*/) {
      setTimeout(function() {
        KTUtil.scrollTop();
      }, 500);
    });
  },
  methods: {
    submit: function(e) {
      e.preventDefault();
      Swal.fire({
        title: "AUTOCCA ",
        text: "Le véhicule a été bien ajouté! {{ fname }}",
        icon: "success",
        confirmButtonClass: "btn btn-secondary"
      });
    },

    addvehicleverifycoherence: function(e) {
      e.preventDefault();
    }
  }
};
</script>
